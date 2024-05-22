---
layout: post
title:  "Recap of AWS Summit Berlin 2024"
date:   2024-05-20 21:04:30 +0200
author: "S3-D1"
tags: [aws, events, automotive]
categories: [dev]
---

# AWS Summit Berlin 2024 - 2024-05-15

> **tl;dr**
>
> The AWS Summit in Berlin was another great experience. Automotive is still growing, and connectivity is increasing. My top three takeaways are:
> - The European Sovereign Cloud - €7.8 billion investment in Brandenburg by the end of 2025
> - GenAI is everywhere - AWS Bedrock and more
> - Karpenter - smart scaling for Kubernetes

<!-- excerpt-end -->

![DALL-E AWS Summit 2024 Berlin Scene]({{ site.baseurl }}/assets/images/2024-05-20-recap-aws-summit.jpg)

Last week, I had the pleasure of attending the AWS Summit in Berlin with my colleague Erik. After a tricky road trip with traffic jams and a hidden hotel parking garage, we arrived just in time for the summit. A quick cup of coffee later, we entered the keynote
area.

Before the keynote started, the atmosphere was set with dim lighting and blue and orange hues preparing the stage. Videos showcasing AWS's efforts played, accompanied by powerful music that energized the audience. The stage was ready for the day's first highlight.

##  Takeaways
### European Sovereign Cloud
One of the most significant announcements on May 15, 2024, was the European Sovereign Cloud. AWS is investing €7.8 billion in Brandenburg by the end of 2025.

With the European Sovereign Cloud, AWS is providing a secure and compliant cloud infrastructure for the European market. This is a great opportunity for German industry and government to advance digital transformation while adhering to European data protection laws. Currently, many companies struggle with data protection laws and cloud compliance. The Patriot Act often conflicts with European laws, and the interconnectedness of regions and availability zones complicates data management. The European Sovereign Cloud aims to eliminate connections to the US and Asian regions or manage them under European governance.

While the benefits for internationally operating German car manufacturers remain to be seen, this initiative is a game changer for German government and national-focused companies. I look forward to seeing amazing digital solutions that will transform daily life, eliminating paper and requiring no more in-person office appointments during working hours.

### GenAI is everywhere
Every talk at the summit mentioned AI, with a wide range of use cases. The topic could fill an entire blog post, and it already has in many places. The internet is flooded with posts, tutorials, and teachings on AI.

The key difference between summit talks and the plethora of online content is AWS's focused approach. All solutions and ideas are driven by AWS, tailored to their customers' use cases, and backed by their technological expertise.

The most impressive use case for me was in cost optimization and utilization improvements of the AWS cloud itself. It's fascinating that AWS is working to reduce their customers' costs, even though it means losing money. Following last year's utilization improvements with Graviton (ARM in AWS), this is a great next step. Karpenter, which I'll discuss next, played a significant role in this optimization.

### Karpenter
Many talks highlighted Karpenter, a smart scaling solution for Kubernetes. This AWS open-source project is still in its early stages but shows great promise. Initially developed in the Cloud Native Foundation, the Autoscaling Special Interest Group (SIG) now works on the project.

At first glance, Karpenter seemed like another autoscaler for Kubernetes. However, its cloud support for AWS sets it apart. Karpenter uses the Fleet API to access information about the availability of different instances, including spot instances. It can then select the most cost-effective available instance, considering capacity to reduce the likelihood of load-based spot instance termination.

The configuration for using this autoscaler is similar to other scalers. The presented cost reductions are impressive, and AWS's efforts to reduce computational waste benefit both customers and the environment. I look forward to my first hands-on experience with Karpenter to see its power firsthand.

## The absence of Automotive DevOps
The summit was fantastic, and I am eager to attend future events, possibly even next year. The quality and quantity of Automotive sessions were excellent, and the audience was broader than last year. I recognize many presented projects from my daily work, and the teams involved should be proud of their progress.

However, I was disappointed by the lack of references to tracetronic, our products, or Automotive DevOps. Automotive DevOps is, in my view, the only viable solution for managing the high volume of code changes in complex, distributed development systems. DevOps cannot be applied to automotive out-of-the-box; it requires significant adaptations. Nonetheless, we are making progress, and the first benefits are already visible. For our vision of continuous software releases for cars, we work with strong partners. Unfortunately, none of them showcased our collaborative innovations at the summit.

My mission for the next year is to change this. By the next summit, I hope to see tracetronic logos prominently displayed. In another year, I want to give a talk on Automotive DevOps, and in three years, I hope to hear our partners or customers presenting on the topic. Meet me at the summit next year, and ask me about our progress. I look forward to it.

