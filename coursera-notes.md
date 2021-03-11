# AWS Cloud Practitioner Essentials

## Module 1: Introduction to Amazon Web Services

### [Video: What is Cloud Computing?](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/CC887/what-is-cloud-computing)

- **Cloud computing:** On-demand delivery of IT resources over the internet with pay-as-you-go pricing.
  - **Cloud-based Deployment:** Migrate or design and build applications in the cloud. Run all parts of the application in the cloud.
  - **On-premises Deployment:** Deploy resources by using virtualization and resource management tools. AKA private cloud deployment. Resources are deployed on premises.
  - **Hybrid Deployment:** Connect cloud-based resources to on-premises infrastructure.
- **Benefits of cloud computing:**
  - Trade upfront expense for variable expense
  - Stop spending money to run and maintain data centers
  - Stop guessing capacity
  - Benefit from massive economies of scale
  - Increase speed and agility (Development and deployment)
  - Go global in minutes

## Module 2: Compute In the Cloud

### [Video: EC2](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/a4gdy/introduction-to-module-2)

- **Amazon Elastic Compute (EC2):** Provides secure, resizable compute capacity in the cloud as Amazon EC2 instances.
- **Multitenancy:** Sharing underlying hardware between virtual machines
- **Vertical scaling:** Make instances bigger or smaller whenever you need to.
- **Amazon EC2 instance types:**
  - **General purpose:** Provides a balance of compute, memory, and networking resources. Used for application servers, gaming servers, backend servers for enterprise applications and small and medium databases.
  - **Compute optimized:** Are ideal for compute-bound applications that benefit from high-performance processors. Ideal for high-performance web servers, compute-intensive applications servers, and dedicated gaming servers. You can also use compute optimized instances for batch processing workloads that require processing many transactions in a single group.
  - **Memory optimized:** Designed to deliver fast performance for workloads that process large datasets in memory.
  - **Accelerated computing:** Use hardware accelerators, or coprocessors, to perform some functions more efficiently than is possible in software running on CPUs. Accelerated computing instances are ideal for workloads such as graphics applications, game streaming, and application streaming.
  - **Storage optimized:** Are designed for workloads that require high, sequential read and write access to large datasets on local storage. Suitable for storage optimized instances include distributed file systems, data warehousing applications, and high-frequency online transaction processing (OLTP) systems.
- **Amazon EC2 Pricing:**

  - **On-Demand:** are ideal for short-term, irregular workloads that cannot be interrupted. No upfront costs or minimum contracts apply. The instances run continuously until you stop them, and you pay for only the compute time you use.
  - **Amazon EC2 Savings Plans:** Enable you to reduce your compute costs by committing to a consistent amount of **compute usage** for a 1-year or 3-year term. Any usage beyond the commitment is charged at regular On-Demand rates.
  - **Reserved Instances:** Are a billing discount applied to the use of On-Demand Instances in your account. You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term, and Scheduled Reserved Instances for a 1-year term.
  - **Spot Instances:** Are ideal for workloads with flexible start and end times, or that can withstand interruptions. Spot Instances use unused Amazon EC2 computing capacity and offer you cost savings at up to 90% off of On-Demand prices.
  - **Dedicated Hosts:** Are physical servers with Amazon EC2 instance capacity that is fully dedicated to your use.

- **Amazon EC2 Auto Scaling:** Enables you to automatically add or remove Amazon EC2 instances in response to changing application demand. You can do this by creating an Auto Scaling group, that allows you to set the minimum number of Amazon EC2 instances. The minimum capacity is the number of Amazon EC2 instances that launch immediately after you have created the Auto Scaling group. In this example, the Auto Scaling group has a minimum capacity of one Amazon EC2 instance.

  - **Dynamic scaling:** Responds to changing demand.
  - **Predictive scaling:** Automatically schedules the right number of Amazon EC2 instances based on predicted demand.

- **Elastic Load Balancer:** Is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances.
- **Decoupled architecture:** Is an architectural approach that allows each computing component to exist and perform tasks independently of one another, while also allowing the components to remain completely unaware and autonomous until instructed
- **Tightly coupled architecture:** All components in the system are linked in such manner that each one is dependent upon each other. **Monolithic Applications** use this approach.
- **Loosely coupled architecture:** Every individual component has no knowledge of the definitions of other components. AKA **Microservices** approach.
- **Amazon Simple Notification Service (SNS):** Is a publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers. In Amazon SNS, subscribers can be web servers, email addresses, AWS Lambda functions, or several other options.
- **Amazon Simple Queue Service (SQS):** Is a message queuing service. It allows you to send, store, and receive messages between software components, without losing messages or requiring other services to be available. In Amazon SQS, an application sends messages into a queue. A user or service retrieves a message from the queue, processes it, and then deletes it from the queue.
- **Payload:** Data contained within a message.
- **Additional Computer Services:**
- **Serverless:** Your code runs on servers, but you do not need to provision or manage these servers.
  - **AWS Lambda:** Is a service that lets you run code without needing to provision or manage servers. You pay only for the compute time that you consume. Charges apply only when your code is running.
- **Containers:** Provide you with a standard way to package your application's code and dependencies into a single object. You can use services such as **Amazon Elastic Container Service (Amazon ECS)**, **Amazon Elastic Kubernetes Service (Amazon EKS)** or **AWS Fargate**.

## Module 3: AWS Global Infrastructure and Reliability

### [Video: Regions](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/pXq5y/regions)

- **Regions:** Are physical locations around the world where data centers are clustered. When determining the right Region for your services, data, and applications, consider the following four business factors.
  - **Compliance** with data governance and legal requirements
  - **Proximity** to your customers
  - **Available** services within a Region
  - **Pricing**
- **Availability Zones:** Is a single data center or a group of data centers within a Region.
- **Edge Locations:** Is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery.
- **Amazon Cloudfront:** Is a fast content delivery network (CDN) service that helps deliver data, video, applications, and APIs to customers around the world with low latency and high transfer speeds. Amazon CloudFront uses Edge locations all around the world to help accelerate communication with users no matter where they are.
- **AWS Outposts:** Is a fully managed service that extends AWS infrastructure, services, APIs, and tools to customer premises. AWS Outposts delivers fully managed AWS infrastructure, native AWS services, APIs, and tools to virtually any customer on premises facility.
- **AWS Resources:**
  - **AWS Management Console:** Is a web-based interface for accessing and managing AWS services.
  - **AWS Command Line Interface (AWS CLI):** Enables you to control multiple AWS services directly from the command line within one tool.
  - **AWS SDKs:** SDKs make it easier for you to use AWS services through an API designed for your programming language or platform. SDKs enable you to use AWS services with your existing applications or create entirely new applications that will run on AWS.
- **AWS Elastic Beanstalk:** Is an easy-to-use service for deploying and scaling web applications and services developed with a variety of programming languages. You provide code and configuration settings, and Elastic Beanstalk deploys the resources necessary to perform the following tasks: Adjust capacity, Load balancing, Automatic scaling, Application health monitoring.
- **AWS CloudFormation:** AWS CloudFormation is an infrastructure as code tool, that allows you to define a wide variety of AWS resources in a declarative way using JSON or YAML text based documents, called CloudFormation Templates.

## Module 4: Networking

### [Video: Conectivity to AWS](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/TdOwH/connectivity-to-aws)

- **Amazon Virtual Private Cloud (Amazon VPC):** Is networking service that you can use to establish boundaries around your AWS resources. Amazon VPC enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within a virtual private cloud (VPC), you can organize your resources into **subnets**. A VPC allows you to define your private IP range for your AWS resources. In a VPC, subnets can communicate with each other. For example, you might have an application that involves Amazon EC2 instances in a public subnet communicating with databases that are located in a private subnet.
- **Subnet:** Subnets are chunks of IP addresses in your VPC that allow you to group resources together. Subnets control whether resources are either publicly, or privately available.
  - **Public Subnet:** Contains resources that need to be accessible by the public, such as an online store’s website.
  - **Private Subnet:** Contains resources that should be accessible only through your private network, such as a database that contains customers’ personal information and order histories.
- **Internet Gateway:** Is a connection between a VPC and the internet to allow public traffic from the internet to access your VPC.
- **Virtual Private Gateway:** The virtual private gateway is the component that allows protected internet traffic to enter into the VPC. A virtual private gateway enables you to establish a virtual private network (VPN) connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.
- **AWS Direct Connect:** Is a service that enables you to establish a dedicated private connection between your data center and a VPC. The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.
- **Packet:** Packets are messages from the internet, and every packet that crosses the subnet boundaries, gets checked against something called a network access control list or Network ACL.
- **Network Access Control List (ACLs):** A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the **subnet level**. By default, **your account’s default network ACL allows all inbound and outbound traffic**, but you can modify it by adding your own rules. For **custom network ACLs, all inbound and outbound traffic is denied** until you add rules to specify which traffic to allow. ACLs are **Stateless**.
  - **Stateless Packet Filtering:** They remember nothing and check packets that cross the subnet border each way: inbound and outbound.
- **Security Group:** A security group is a virtual firewall that controls inbound and outbound traffic for an **Amazon EC2 instance**. By default, a security group **denies all inbound traffic and allows all outbound traffic**. You can add custom rules to configure which traffic to allow or deny. Security Groups are **Stateful**.
  - **Stateful Packet Filtering:** They remember previous decisions made for incoming packets.
- **Amazon Route 53:** Is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS. Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS. Another feature of Route 53 is the ability to manage the DNS records for domain names.

## Module 5: Storage and databases

### [Video: Storage and databases](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/A3izm/introduction-to-module-5)

- Block level storage
- Instance store volumes
- Amazon Elastic Block Store (EBS)
- EBS Volumes
- Snapshots: Incremental backups
- Amazon Simple Storage Service (S3)
  - Standard
  - Static website hosting
  - Stardard Infrequent Access (Standard I-A)
  - S3 Intelligent-Tiering
  - S3 Glacier
  - S3 Glacier Deep Archive
- Amazon Elastic File (EFS)
- Amazon Relational Database Service
- Amazon Aurora
- Amazon DynamoDB
- Amazon Redshift
- AWS Database Migration Service (AWS DMS)
  - Homogeneous databases
  - Heterogeneous databases'
  - Development and test database migrations
  - Database consolidation
  - Continuous replication
- Amazon DocumentDB (MongoDB Compability)
- Amazon Neptune
- Amazon Managed Blockchain
- Amazon Quantum Ledger Database
- Database Accelerator
- Amazon ElastiCache
- Amazon DynamoDB Accelerator (DAX)

## Module 6: Security

### [Video: Security](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/boUyb/introduction-to-module-6)

- AWS Responsibility model
- AWS account root user
  - MFA
- AWS Identity an Access Management (AWS IAM)
- Principle of least privilege
- IAM Policy
- IAM Groups
- IAM Role
- Identity Federation
- AWS Organizations
  - Centralized Management
  - Consolidated billing
  - Hierarchical groupings of accounts
  - AWS servvices and API actions access control
  - Service control policies (SPCs)
- AWS Compliance
- AWS Artifact
  - AWS Artifact Agreements
  - AWS Artifact Reports
- Customer Compliance Center
- Distributed Denial-of-service (DDoS)
  - UDP Flood
  - HTTP Level attacks
  - SLow loris attack
- AWS Shield
  - Standard
  - Advanced
- AWS WAF
- Encryption at reset
- Encryption In-transit
- AWS Key Management Service (AWS KMS)
- Amazon Inspector
- Amazon GuardDuty

## Module 7: Monitoring and Analytics

### [Video: Monitoring and Analytics](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/Fn2nN/introduction-to-module-7)

- Amazon CloudWatch
  - Amazon CloudWatch Alarm
  - MTTR & TCO
- AWS CloudTrail
- CloudTrail Insights
- AWS Trusted Advisor

## Module 8: Pricing and Support

### [Video: Pricing and Support](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/DdiEO/introduction-to-module-8)

- AWS Free Tier
- AWS Pricing
- Billing Dashboard
- Consolidated Billing
- AWS Budgets
- AWS Cost Explorer
- AWS Console Billing
- AWS Support Plans
  - Basic
  - Developer
  - Business
  - Enterprise
- AWS Personal Health Dashboard
- Technical Account Manager (TAM)
- AWS Marketplace

## Module 9: Migration and Innovation

### [Video: Migration and Innovation](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/DaXvL/introduction-to-module-9)

- AWS Cloud Adoption Framework (AWS CAF)
  - AWS CAF Perspectives
  - AWS CAF Action Plan
- 6 R's of Migration
  - Rehosting
  - Replatforming
  - Retire
  - Retain
  - Repurchase
  - Refactor
- AWS Snow Family
  - AWS Snowcone
  - AWS Snowball Edge
    - Storage Optimized
    - Compute Optimized
  - AWS Snowmobile
- Amazon SageMaker
- Amazon Augmented AI (Amazon A2I)
- Amazon Lex
- Amazon Textract
- Amazon DeepRacer
- Internet of Things
- AWS Ground Station

## Module 10: The Cloud Journey

### [Video: The Cloud Journey](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/MiAby/introduction-to-module-10)

- AWS Well-Architected Framework
- Benefits of the AWS Cloud

## AWS Certified Cloud Practicioner Basics

### [Exam Details](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/supplement/GQ6hE/exam-details)
