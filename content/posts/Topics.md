---
title: Variety of Topics
description: Sed ut perspiciatis unde omnis iste natus error sit voluptatem
date: 2015-09-08
tags:
- Lorem
- Ipsum
draft: false

---
## Cloud Computing

### Serverless Computing

Jonas, E., Schleier-Smith, J., Sreekanti, V., Tsai, C. C., Yadwadkar, N., Gonzalez, J. E., Popa, R. A., Stoica, I., & Patterson, D. A. (2019). Serverless computing: One step forward, two steps back. Proceedings of the 10th ACM Symposium on Cloud Computing, 1-13. https://doi.org/10.1145/3357223.3362700

Cloud services are multitenant and easier-to-manage versions of enterprise data storage ie object storage, databases, queueing systems, and web/app servers. But this only scratches the surface of its potential, with millions of cores and exabytes of data. 

Serverless computing allows developers to upload their code and only pay when it is run. 

“Serverless” goes FaaS
Functions-as-a-Service (FaaS) is a core part of serverless offerings including AWS Lambda, Azure and Google Cloud Platform. 

Functions map inputs to outputs. Functions are triggered by events. Infrastructure monitors events, runs the functions, and stores results. Users are only billed for the resources they use. 

FaaS are not efficient for data processing tasks because of the cold start latency, where the cloud provider must start the runtime environment. Faas are ephmemeral, or they are stateless and short-lived whereas data processing needs to be state managed. Functions have memory and CPU limits. FaaS need data movement, which can cause latency. 

Faas are not well suited for distributed systems. 
Faas functions are stateless, whereas distributed systems require statefull processing. Also they are complex and communicate frequently. 


Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?
