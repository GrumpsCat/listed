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

Greenberg, Albert, et al. "The cost of a cloud: research problems in data center networks." ACM SIGCOMM computer communication review 39.1 (2008): 68-73.

The paper explores the cost structure of cloud service data centers and identifies areas where research and development (R&D) can significantly impact cost efficiency and performance. The authors analyze the amortized costs associated with data centers and propose solutions to optimize these costs.

#### Key Components of Data Center Costs

The cost components of data centers are broken down into the following categories:

1. **Servers (∼45%)**: This includes the cost of CPUs, memory, and storage systems.
2. **Infrastructure (∼25%)**: This covers power distribution and cooling systems.
3. **Power Draw (∼15%)**: This involves the electrical utility costs to run the servers.
4. **Network (∼15%)**: This includes the cost of network links, transit, and equipment.

#### Main Challenges and Proposed Solutions

1. **Resource Utilization**:
   - **Problem**: Data centers often operate at low utilization due to resource stranding and fragmentation.
   - **Solution**: Increase network agility and provide appropriate incentives to shape resource consumption.

2. **Geo-Distributed Networks**:
   - **Problem**: Building out geo-distributed networks of data centers can raise the cost of providing service without appropriate design and management.
   - **Solution**: Joint optimization of network and data center resources, and new systems and mechanisms for geo-distributing state.

### Detailed Explanation

#### 1. Introduction to Cloud Service Data Centers

Large companies like eBay, Facebook, Google, Microsoft, and Yahoo! have made significant investments in massive data centers to support cloud services. The paper investigates the costs associated with these data centers and identifies opportunities for R&D to reduce costs and improve efficiency.

#### 2. Breakdown of Data Center Costs

The authors provide a cost breakdown for a data center with approximately 50,000 servers, highlighting the importance of optimizing work completed per dollar invested.

#### 3. Differences Between Enterprise and Cloud Service Data Centers

- **Operational Staff Costs**: In enterprise data centers, operational staff costs are significant. In cloud service data centers, automation reduces these costs to under 5%.
- **Economies of Scale**: Cloud service data centers benefit from economies of scale, which are not present in enterprise data centers.
- **Scale Out vs. Scale Up**: Enterprises optimize for physical space and device count by consolidating workloads onto a few high-cost servers. Cloud service data centers distribute workloads across many low-cost servers.

#### 4. Types of Cloud Service Data Centers

- **Mega Data Centers**: These house tens of thousands of servers, suitable for applications requiring massive computational resources.
- **Micro Data Centers**: These contain thousands of servers and are located close to major population centers to minimize latency and network transit costs.

### Importance of Networking and Systems Innovation

While networking is not the largest cost component, innovations in networking and systems are crucial for reducing overall costs and improving efficiency. The authors argue that optimizing the network can significantly enhance the performance and cost-effectiveness of data centers.

Sure, let's delve into Section 2 of the paper "The Cost of a Cloud: Research Problems in Data Center Networks" and break down the cost components of a data center as described by the authors.

### Section 2: Cost Breakdown

The authors provide a detailed analysis of the costs associated with running a cloud service data center. Each cost component is discussed in terms of its impact and potential for optimization. The main cost components analyzed are servers, infrastructure, power, and network.

#### 2.1 Server Cost

**Servers** constitute the largest cost in a data center, accounting for about 45% of the total cost. For example, if a data center has 50,000 servers, each costing $3000, with a 5% cost of money and a 3-year amortization period, the amortized cost of servers is approximately $52.5 million per year.

**Challenges in Server Utilization**:
- **Uneven Application Fit**: Servers integrate CPU, memory, network, and storage components. Often, applications do not fully utilize all these components, leading to inefficient resource use.
- **Uncertainty in Demand Forecasts**: Cloud service demands can spike unexpectedly, making it difficult to forecast and provision resources accurately.
- **Long Provisioning Time Scales**: Server purchases are usually made in bulk and intended to last several years, which complicates the ability to respond quickly to changes in demand.
- **Risk Management**: To avoid service failure during demand spikes, there is a tendency to over-provision resources.
- **Hoarding**: Service teams may be reluctant to return unused resources, leading to inefficiencies.
- **Virtualization Shortfalls**: While virtualization helps in moving processes between machines, network constraints can still hinder resource agility.

**Reducing Server Costs**:
To improve server utilization, the key is **agility**—the ability to dynamically allocate and deallocate resources to meet demand. Enhancing network capabilities to reduce fragmentation and increase flexibility is crucial. The authors suggest that solving these issues requires a more agile network infrastructure, which is discussed further in Section 3.

#### 2.2 Infrastructure Cost

**Infrastructure** costs, which include power delivery and cooling systems, represent about 25% of the total cost. These costs involve significant capital investments in generators, transformers, and Uninterruptible Power Supply (UPS) systems.

**Infrastructure Components**:
- Power from the utility is transformed and delivered to the servers.
- In case of long-term outages, generators keep the data center operational.

With typical infrastructure costs of $200 million, a 5% cost of money, and a 15-year amortization period, the annual cost of infrastructure is approximately $18.4 million.

**Reducing Infrastructure Costs**:
One approach is to **relax the requirement for consistent power delivery** at the individual server level. Instead of building highly resilient data centers, the authors propose using larger numbers of smaller data centers with a 1:N resilience model, where the failure unit becomes the entire data center. This approach could eliminate the need for costly redundancy within each data center, such as UPS and generators. Designing strategies for balancing resilience within and across data centers is a rich area for research.

#### 2.3 Power Cost

**Power** costs account for about 15% of the total. Using state-of-the-art facilities with a Power Usage Efficiency (PUE) of 1.7, and assuming a utility price of $0.07 per KWH, the total power cost for 50,000 servers (each drawing an average of 180W) is approximately $9.3 million per year.

**Reducing Power Costs**:
To reduce power costs, focus on:
- **Improving Server Energy Efficiency**: Hardware innovations, such as high-efficiency power supplies and voltage regulation modules, can help.
- **Energy Proportionality**: Servers should consume power proportional to their load.
- **Running Data Centers Hotter**: Reducing cooling needs by allowing higher operating temperatures can save on cooling costs, but requires research into hardening equipment against higher failure rates.

#### 2.4 Network Cost

**Network** costs represent about 15% of the total. This includes the cost of networking gear like switches, routers, and load balancers, as well as wide area networking costs for peering, inter-data center links, and regional facilities.

**Reducing Network Costs**:
- **Optimizing Site Selection and Peering Strategies**: Clever design of peering and transit strategies and optimal placement of data centers can reduce costs.
- **Optimizing Service Design**: Partitioning functionality and state between data centers and designing better methods for managing traffic and mapping users to data centers can reduce network costs.

#### 2.5 Perspective

The authors emphasize two main rules of thumb:
1. **On is Better than Off**: Maximizing server utilization by ensuring servers are engaged in revenue-producing activity.
2. **Build in Resilience at the Systems Level**: Reducing infrastructure costs by eliminating redundancy within each data center and achieving resilience through multiple data centers.

To tackle the challenges of low utilization and high latency, the paper highlights the need for:
- Better mechanisms for increasing network agility.
- Providing appropriate incentives to shape resource consumption.
- Joint optimization of network and data center resources.
- New systems and mechanisms for geo-distributing state.







---

### Serverless Computing

`Jonas, E., Schleier-Smith, J., Sreekanti, V., Tsai, C. C., Yadwadkar, N., Gonzalez, J. E., Popa, R. A., Stoica, I., & Patterson, D. A. (2019). Serverless computing: One step forward, two steps back. Proceedings of the 10th ACM Symposium on Cloud Computing, 1-13. https://doi.org/10.1145/3357223.3362700`

Cloud services are multitenant and easier-to-manage versions of enterprise data storage ie object storage, databases, queueing systems, and web/app servers. But this only scratches the surface of its potential, with millions of cores and exabytes of data.

Serverless computing allows developers to upload their code and only pay when it is run. 

**1 INTRODUCTION**
“Serverless” goes FaaS
Functions-as-a-Service (FaaS) is a core part of serverless offerings including AWS Lambda, Azure and Google Cloud Platform. 

Functions map inputs to outputs. Functions are triggered by events. Infrastructure monitors events, runs the functions, and stores results. Users are only billed for the resources they use. 

FaaS are not efficient for data processing tasks because of the cold start latency, where the cloud provider must start the runtime environment. Faas are ephmemeral, or they are stateless and short-lived whereas data processing needs to be state managed. Functions have memory and CPU limits. FaaS need data movement, which can cause latency. 

Faas are not well suited for distributed systems. 
Faas functions are stateless, whereas distributed systems require statefull processing. Also they are complex and communicate frequently. 

**2 SERVERLESS IS MORE? THE EASY CASES**
FaaS are great for simple, parallel tasks with long latency times. This limits the attractiveness of FaaS. 

**3 WHY SERVERLESS TODAY IS TOO LESS**
Cloud services offer unlimited data storage and unlimited distributed computing power. 
Where:
Function limited lifetimes, bandwidth limitations, slow communications and no specalized hardware. 

---