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

- Regions
- Availability Zones
- Edge Locations
- Amazon Cloudfront
- Amazon Route 53
- AWS Outposts
- AWS Resources
  - AWS Management Console
  - AWS CLI
  - AWS SDKs
- AWS Elastic Beanstalk
- AWS CloudFormation

## Module 4: Networking

### [Video: Conectivity to AWS](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/TdOwH/connectivity-to-aws)

- VPC
- Subnet
- Internet Gateway
- Virtual Private Gateway
- AWS Direct Connect
- Network Hardening
- Packet
- Network Access control list
  - Stateless
- Security Group
  - Stateful
- Amazon Route 53

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
