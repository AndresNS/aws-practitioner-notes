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

- **Block level storage:** Is a place to store files, whereas a file is a series of bytes that are stored in blocks on disk. When a file is updated, the whole series of blocks aren't all overwritten. Instead, it updates just the pieces that change.
- **Instance store volumes:** Some EC2 instances come with a local storage called instance store volumes. These volumes are physically attached to the host your EC2 instance is running on top of, and you can write to it just like a normal hard drive. However, since this volume is attached to the underlying physical host, if you stop or terminate your EC2 instance, all data written to the instance store volume will be deleted.
- **Amazon Elastic Block Store (Amazon EBS):** Is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available. Because EBS volumes are for data that needs to persist, it’s important to back up the data. You can take incremental backups of EBS volumes by creating **Amazon EBS snapshots**. Sizes up to 16 TiB.
- **Amazon EBS snapshots:** Is an incremental backup. This means that the first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.
- **Object Storage:** In object storage, each object consists of data, metadata, and a key. The data might be an image, video, text document, or any other type of file. Metadata contains information about what the data is, how it is used, the object size, and so on. An object’s key is its unique identifier. Unlike Block Level Storage, when a file in object storage is modified, the entire object is updated.
- **Amazon Simple Storage Service (S3):** Is a service that provides object-level storage. Amazon S3 stores data as objects in buckets. You can upload any type of file to Amazon S3, such as images, videos, text files, and so on. Amazon S3 offers unlimited storage space. The maximum file size for an object in Amazon S3 is 5 TB. When you upload a file to Amazon S3, you can set permissions to control visibility and access to it. You can also use the Amazon S3 versioning feature to track changes to your objects over time.
  - **Standard:** Designed for frequently accessed data. Stores data in a minimum of three Availability Zones. S3 Standard provides high availability for objects. This makes it a good choice for a wide range of use cases, such as websites, content distribution, and data analytics. S3 Standard has a higher cost than other storage classes intended for infrequently accessed data and archival storage.
  - **S3 Standard-Infrequent Access (S3 Standard-IA):** S3 Standard-IA is ideal for data infrequently accessed but requires high availability when needed. Both S3 Standard and S3 Standard-IA store data in a minimum of three Availability Zones. S3 Standard-IA provides the same level of availability as S3 Standard but with a lower storage price and a higher retrieval price.
  - **S3 One Zone-Infrequent Access (S3 One Zone-IA):** Compared to S3 Standard and S3 Standard-IA, which store data in a minimum of three Availability Zones, S3 One Zone-IA stores data in a single Availability Zone. This makes it a good storage class to consider if the following conditions apply:
    - You want to save costs on storage.
    - You can easily reproduce your data in the event of an Availability Zone failure.
  - **S3 Intelligent-Tiering:** Ideal for data with unknown or changing access patterns. Requires a small monthly monitoring and automation fee per object. In the S3 Intelligent-Tiering storage class, Amazon S3 monitors objects’ access patterns. If you haven’t accessed an object for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, S3 Standard-IA. If you access an object in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, S3 Standard.
  - **S3 Glacier:** Low-cost storage designed for data archiving. Able to retrieve objects within a few minutes to hours. S3 Glacier is a low-cost storage class that is ideal for data archiving. For example, you might use this storage class to store archived customer records or older photos and video files.
  - **S3 Glacier Deep Archive:** Lowest-cost object storage class ideal for archiving. Able to retrieve objects within 12 hours. When deciding between Amazon S3 Glacier and Amazon S3 Glacier Deep Archive, consider how quickly you need to retrieve archived objects. You can retrieve objects stored in the S3 Glacier storage class within a few minutes to a few hours. By comparison, you can retrieve objects stored in the S3 Glacier Deep Archive storage class within 12 hours.
- **File Storage:** In file storage, multiple clients (such as users, applications, servers, and so on) can access data that is stored in shared file folders. In this approach, a storage server uses block storage with a local file system to organize files. Clients access data through file paths. Compared to block storage and object storage, file storage is ideal for use cases in which a large number of services and resources need to access the same data at the same time.
- **Amazon Elastic File System (Amazon EFS):** Is a scalable file system used with AWS Cloud services and on-premises resources. As you add and remove files, Amazon EFS grows and shrinks automatically. It can scale on demand to petabytes without disrupting applications. Amazon EFS is a regional service. It stores data in and across multiple Availability Zones. The duplicate storage enables you to access data concurrently from all the Availability Zones in the Region where a file system is located. Additionally, on-premises servers can access Amazon EFS using AWS Direct Connect.
- **Amazon Relational Database Service (Amazon RDS):** Is a service that enables you to run relational databases in the AWS Cloud. Amazon RDS is available on six database engines, which optimize for memory, performance, or input/output (I/O). Supported database engines include: Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database, Microsoft SQL Server.
- **Amazon Aurora:** Is an enterprise-class relational database. It is compatible with MySQL and PostgreSQL relational databases. It is up to five times faster than standard MySQL databases and up to three times faster than standard PostgreSQL databases. Amazon Aurora helps to reduce your database costs by reducing unnecessary input/output (I/O) operations, while ensuring that your database resources remain reliable and available. Consider Amazon Aurora if your workloads require high availability. It replicates six copies of your data across three Availability Zones and continuously backs up your data to Amazon S3.
- **Amazon DynamoDB:** Is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. 
- **Amazon Redshift:** Is a data warehousing service that you can use for big data analytics. It offers the ability to collect data from many sources and helps you to understand relationships and trends across your data.
- **AWS Database Migration Service (AWS DMS):** Enables you to migrate relational databases, nonrelational databases, and other types of data stores. With AWS DMS, you move data between a source database and a target database. The source and target databases can be of the same type or different types. During the migration, your source database remains operational, reducing downtime for any applications that rely on the database.
  - **Homogeneous databases:** Is when the schema structures, data types, and database code is compatible between source and target.
  - **Heterogeneous databases:** Is a type of migration in which source and target databases are of different types. Since the schema structures, data types, and database code are different between source and target, it is necessary to convert them using the AWS schema conversion tool.
  - Other use cases for AWS DMS are: 
    - **Development and test database migrations:** Enabling developers to test applications against production data without affecting production users.
    - **Database consolidation:** Combining several databases into a single database.
    - **Continuous replication:** Sending ongoing copies of your data to other target sources instead of doing a one-time migration.
- **Additional Database Services:**
  - **Amazon DocumentDB:** Is a document database service that supports MongoDB workloads. (MongoDB is a document database program.)
  - **Amazon Neptune:** Is a graph database service. You can use Amazon Neptune to build and run applications that work with highly connected datasets, such as recommendation engines, fraud detection, and knowledge graphs.
  - **Amazon Managed Blockchain:** Is a service that you can use to create and manage blockchain networks with open-source frameworks. Blockchain is a distributed ledger system that lets multiple parties run transactions and share data without a central authority.
  - **Amazon Quantum Ledger Database (Amazon QLDB) :** Is a ledger database service. You can use Amazon QLDB to review a complete history of all the changes that have been made to your application data.
  - **Database Accelerator:**
    - **Amazon ElastiCache:** Is a service that adds caching layers on top of your databases to help improve the read times of common requests. It supports two types of data stores: Redis and Memcached.
    - **Amazon DynamoDB Accelerator (DAX):** Is an in-memory cache for DynamoDB. 

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
