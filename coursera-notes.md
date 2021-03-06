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
  - **Public Subnet:** Contains resources that need to be accessible by the public, such as an online store???s website.
  - **Private Subnet:** Contains resources that should be accessible only through your private network, such as a database that contains customers??? personal information and order histories.
- **Internet Gateway:** Is a connection between a VPC and the internet to allow public traffic from the internet to access your VPC.
- **Virtual Private Gateway:** The virtual private gateway is the component that allows protected internet traffic to enter into the VPC. A virtual private gateway enables you to establish a virtual private network (VPN) connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.
- **AWS Direct Connect:** Is a service that enables you to establish a dedicated private connection between your data center and a VPC. The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.
- **Packet:** Packets are messages from the internet, and every packet that crosses the subnet boundaries, gets checked against something called a network access control list or Network ACL.
- **Network Access Control List (ACLs):** A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the **subnet level**. By default, **your account???s default network ACL allows all inbound and outbound traffic**, but you can modify it by adding your own rules. For **custom network ACLs, all inbound and outbound traffic is denied** until you add rules to specify which traffic to allow. ACLs are **Stateless**.
  - **Stateless Packet Filtering:** They remember nothing and check packets that cross the subnet border each way: inbound and outbound.
- **Security Group:** A security group is a virtual firewall that controls inbound and outbound traffic for an **Amazon EC2 instance**. By default, a security group **denies all inbound traffic and allows all outbound traffic**. You can add custom rules to configure which traffic to allow or deny. Security Groups are **Stateful**.
  - **Stateful Packet Filtering:** They remember previous decisions made for incoming packets.
- **Amazon Route 53:** Is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS. Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS. Another feature of Route 53 is the ability to manage the DNS records for domain names.

## Module 5: Storage and databases

### [Video: Storage and databases](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/A3izm/introduction-to-module-5)

- **Block level storage:** Is a place to store files, whereas a file is a series of bytes that are stored in blocks on disk. When a file is updated, the whole series of blocks aren't all overwritten. Instead, it updates just the pieces that change.
- **Instance store volumes:** Some EC2 instances come with a local storage called instance store volumes. These volumes are physically attached to the host your EC2 instance is running on top of, and you can write to it just like a normal hard drive. However, since this volume is attached to the underlying physical host, if you stop or terminate your EC2 instance, all data written to the instance store volume will be deleted.
- **Amazon Elastic Block Store (Amazon EBS):** Is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available. Because EBS volumes are for data that needs to persist, it???s important to back up the data. You can take incremental backups of EBS volumes by creating **Amazon EBS snapshots**. Sizes up to 16 TiB.
- **Amazon EBS snapshots:** Is an incremental backup. This means that the first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.
- **Object Storage:** In object storage, each object consists of data, metadata, and a key. The data might be an image, video, text document, or any other type of file. Metadata contains information about what the data is, how it is used, the object size, and so on. An object???s key is its unique identifier. Unlike Block Level Storage, when a file in object storage is modified, the entire object is updated.
- **Amazon Simple Storage Service (S3):** Is a service that provides object-level storage. Amazon S3 stores data as objects in buckets. You can upload any type of file to Amazon S3, such as images, videos, text files, and so on. Amazon S3 offers unlimited storage space. The maximum file size for an object in Amazon S3 is 5 TB. When you upload a file to Amazon S3, you can set permissions to control visibility and access to it. You can also use the Amazon S3 versioning feature to track changes to your objects over time.
  - **Standard:** Designed for frequently accessed data. Stores data in a minimum of three Availability Zones. S3 Standard provides high availability for objects. This makes it a good choice for a wide range of use cases, such as websites, content distribution, and data analytics. S3 Standard has a higher cost than other storage classes intended for infrequently accessed data and archival storage.
  - **S3 Standard-Infrequent Access (S3 Standard-IA):** S3 Standard-IA is ideal for data infrequently accessed but requires high availability when needed. Both S3 Standard and S3 Standard-IA store data in a minimum of three Availability Zones. S3 Standard-IA provides the same level of availability as S3 Standard but with a lower storage price and a higher retrieval price.
  - **S3 One Zone-Infrequent Access (S3 One Zone-IA):** Compared to S3 Standard and S3 Standard-IA, which store data in a minimum of three Availability Zones, S3 One Zone-IA stores data in a single Availability Zone. This makes it a good storage class to consider if the following conditions apply:
    - You want to save costs on storage.
    - You can easily reproduce your data in the event of an Availability Zone failure.
  - **S3 Intelligent-Tiering:** Ideal for data with unknown or changing access patterns. Requires a small monthly monitoring and automation fee per object. In the S3 Intelligent-Tiering storage class, Amazon S3 monitors objects??? access patterns. If you haven???t accessed an object for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, S3 Standard-IA. If you access an object in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, S3 Standard.
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

- **AWS Responsibility model:** Customers are responsible for the security of everything that they create and put in the AWS Cloud: Operating System, Application, Data. AWS is responsible for security of the cloud: Physical, Network, Hypervisor
- **AWS account root user:** Owner of the AWS account. The root user is accessed by signing in with the email address and password that you used to create your AWS account. It has complete access to all the AWS services and resources in the account.

  - **MFA:** Multi-factor authentication. In IAM, multi-factor authentication (MFA) provides an extra layer of security for your AWS account.

- **AWS Identity an Access Management (AWS IAM):** Enables you to manage access to AWS services and resources securely.
- **Principle of least privilege:** A user is granted access only to what they need.
- **IAM User** An IAM user is an identity that you create in AWS. It represents the person or application that interacts with AWS services and resources. It consists of a name and credentials. By default, when you create a new IAM user in AWS, it has no permissions associated with it.
- **IAM Policy:** An IAM policy is a document that allows or denies permissions to AWS services and resources.
- **IAM Groups:** An IAM group is a collection of IAM users. When you assign an IAM policy to a group, all users in the group are granted permissions specified by the policy.
- **IAM Role:** An IAM role is an identity that you can assume to gain temporary access to permissions.
- **Identity Federation:**
- **AWS Organizations:** AWS Organizations helps you centrally manage and govern your environment as you grow and scale your AWS resources.
  - Centralized Management
  - Consolidated billing
  - Hierarchical groupings of accounts
  - AWS services and API actions access control
  - **Service control policies (SPCs):** Service control policies (SCPs) are a type of organization policy that you can use to manage permissions in your organization.
- **AWS Artifact:** AWS Artifact is a service that provides on-demand access to AWS security and compliance reports and select online agreements. AWS Artifact consists of two main sections: AWS Artifact Agreements and AWS Artifact Reports.
  - **AWS Artifact Agreements:** In AWS Artifact Agreements, you can review, accept, and manage agreements for an individual account and for all your accounts in AWS Organizations.
  - **AWS Artifact Reports:** AWS Artifact Reports provide compliance reports from third-party auditors. These auditors have tested and verified that AWS is compliant with a variety of global, regional, and industry-specific security standards and regulations.
- **Customer Compliance Center:** In the Customer Compliance Center, you can read customer compliance stories to discover how companies in regulated industries have solved various compliance, governance, and audit challenges.
- **Distributed Denial-of-service (DDoS):** In a distributed denial-of-service (DDoS) attack, multiple sources are used to start an attack that aims to make a website or application unavailable. This can come from a group of attackers, or even a single attacker.
  - **UDP Flood:** Security Groups
  - **HTTP Level attacks:**
  - **SLowloris attack:** ELB
- **AWS Shield:** AWS Shield is a service that protects applications against DDoS attacks. AWS Shield provides two levels of protection: Standard and Advanced.
  - **Standard:** Automatically protects all AWS customers at no cost. It protects your AWS resources from the most common, frequently occurring types of DDoS attack.
  - **Advanced:** Is a paid service that provides detailed attack diagnostics and the ability to detect and mitigate sophisticated DDoS attacks. Additionally, you can integrate AWS Shield with AWS WAF by writing custom rules to mitigate complex DDoS attacks.
- **AWS WAF:** AWS WAF is a web application firewall that helps protect your web applications or APIs against common web exploits that may affect availability, compromise security, or consume excessive resources. AWS WAF works together with Amazon CloudFront and an Application Load Balancer. AWS WAF blocks or allows traffic by using a web access control list (ACL) to protect your AWS resources.
- **AWS Key Management Service (AWS KMS):** Enables you to perform encryption operations through the use of cryptographic keys. You can use AWS KMS to create, manage, and use cryptographic keys. You can also control the use of keys across a wide range of services and in your applications.
- **Amazon Inspector:** Amazon Inspector helps to improve the security and compliance of applications by running automated security assessments.
- **Amazon GuardDuty:** Is a service that provides intelligent threat detection for your AWS infrastructure and resources. It identifies threats by continuously monitoring the network activity and account behavior within your AWS environment.

## Module 7: Monitoring and Analytics

### [Video: Monitoring and Analytics](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/Fn2nN/introduction-to-module-7)

- **Amazon CloudWatch:** Is a web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics.
  - **Amazon CloudWatch Alarm:** With CloudWatch, you can create alarms that automatically perform actions if the value of your metric has gone above or below a predefined threshold.
- **AWS CloudTrail:** AWS CloudTrail records API calls for your account. The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more.
- **CloudTrail Insights:** This optional feature allows CloudTrail to automatically detect unusual API activities in your AWS account.
- **AWS Trusted Advisor:** Is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices. Trusted Advisor compares its findings to AWS best practices in five categories: cost optimization, performance, security, fault tolerance, and service limits.

## Module 8: Pricing and Support

### [Video: Pricing and Support](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/DdiEO/introduction-to-module-8)

- **AWS Free Tier:** The AWS Free Tier enables you to begin using certain services without having to worry about incurring costs for the specified period.
  - **Always Free:** These offers do not expire and are available to all AWS customers.
  - **12 months Free:** These offers are free for 12 months following your initial sign-up date to AWS.
  - **Trials:** Short-term free trial offers start from the date you activate a particular service. The length of each trial might vary by number of days or the amount of usage in the service.
  - **Free Services:** SageMaker, Comprehend Medical, DynamoDB, SNS, Cognito
- **AWS Pricing:**
  - Pay for what you use.
  - Pay less when you reserve.
  - Pay less with volume-based discounts when you use more.
- **AWS Pricing Calculator:** The AWS Pricing Calculator lets you explore AWS services and create an estimate for the cost of your use cases on AWS. You can organize your AWS estimates by groups that you define.
- **Billing Dashboard:** Use the AWS Billing & Cost Management dashboard to pay your AWS bill, monitor your usage, and analyze and control your costs.
  - Publish AWS Cost and Usage Reports.
- **Consolidated Billing:** The consolidated billing feature of AWS Organizations enables you to receive a single bill for all AWS accounts in your organization. By consolidating, you can easily track the combined costs of all the linked accounts in your organization. The default maximum number of accounts allowed for an organization is 4, but you can contact AWS Support to increase your quota, if needed.
- **AWS Budgets:** In AWS Budgets, you can create budgets to plan your service usage, service costs, and instance reservations. In AWS Budgets, you can also set custom alerts when your usage exceeds (or is forecasted to exceed) the budgeted amount.
- **AWS Cost Explorer:** AWS Cost Explorer is a tool that enables you to visualize, understand, and manage your AWS costs and usage over time.
- **AWS Console Billing:**
- **AWS Support Plans:**
  - **Basic:** Basic Support is free for all AWS customers. It includes access to whitepapers, documentation, and support communities. With Basic Support, you can also contact AWS for billing questions and service limit increases. With Basic Support, you have access to a limited selection of AWS Trusted Advisor checks. Additionally, you can use the **AWS Personal Health Dashboard**, a tool that provides alerts and remediation guidance when AWS is experiencing events that may affect you.
  - **Developer:** Best practice guidance. Client-side diagnostic tools. Building-block architecture support, which consists of guidance for how to use AWS offerings, features, and services together.
  - **Business:** Use-case guidance to identify AWS offerings, features, and services that can best support your specific needs. All AWS Trusted Advisor checks. Limited support for third-party software, such as common operating systems and application stack components.
  - **Enterprise:** Application architecture guidance, which is a consultative relationship to support your company???s specific use cases and applications. Infrastructure event management: A short-term engagement with AWS Support that helps your company gain a better understanding of your use cases. This also provides your company with architectural and scaling guidance. A Technical Account Manager
- **Technical Account Manager (TAM):** If your company has an Enterprise Support plan, the TAM is your primary point of contact at AWS. They provide guidance, architectural reviews, and ongoing communication with your company as you plan, deploy, and optimize your applications. Your TAM provides expertise across the full range of AWS services. They help you design solutions that efficiently use multiple services together through an integrated approach.
- **AWS Marketplace:** AWS Marketplace is a digital catalog that includes thousands of software listings from independent software vendors. You can use AWS Marketplace to find, test, and buy software that runs on AWS.

## Module 9: Migration and Innovation

### [Video: Migration and Innovation](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/DaXvL/introduction-to-module-9)

- **AWS Cloud Adoption Framework (AWS CAF):** At the highest level, the AWS Cloud Adoption Framework (AWS CAF) organizes guidance into six areas of focus, called Perspectives. Each Perspective addresses distinct responsibilities. The planning process helps the right people across the organization prepare for the changes ahead.
  - **AWS CAF Perspectives:** In general, the Business, People, and Governance Perspectives focus on business capabilities, whereas the Platform, Security, and Operations Perspectives focus on technical capabilities.
    - **Business:** The Business Perspective ensures that IT aligns with business needs and that IT investments link to key business results. Use the Business Perspective to create a strong business case for cloud adoption and prioritize cloud adoption initiatives. Ensure that your business strategies and goals align with your IT strategies and goals.
    - **People:** The People Perspective supports development of an organization-wide change management strategy for successful cloud adoption. Use the People Perspective to evaluate organizational structures and roles, new skill and process requirements, and identify gaps. This helps prioritize training, staffing, and organizational changes.
    - **Governance:** Use the Governance Perspective to understand how to update the staff skills and processes necessary to ensure business governance in the cloud. Manage and measure cloud investments to evaluate business outcomes.
    - **Platform:** The Platform Perspective includes principles and patterns for implementing new solutions on the cloud, and migrating on-premises workloads to the cloud. Use a variety of architectural models to understand and communicate the structure of IT systems and their relationships. Describe the architecture of the target state environment in detail.
    - **Security:** The Security Perspective ensures that the organization meets security objectives for visibility, auditability, control, and agility. Use the AWS CAF to structure the selection and implementation of security controls that meet the organization???s needs.
    - **Operations:** The Operations Perspective helps you to enable, run, use, operate, and recover IT workloads to the level agreed upon with your business stakeholders. Define how day-to-day, quarter-to-quarter, and year-to-year business is conducted. Align with and support the operations of the business. The AWS CAF helps these stakeholders define current operating procedures and identify the process changes and training needed to implement successful cloud adoption.
- **6 R's of Migration:** When migrating applications to the cloud, six of the most common migration strategies that you can implement are:
  - **Rehosting:** Also known as ???lift-and-shift??? involves moving applications without changes. In the scenario of a large legacy migration, in which the company is looking to implement its migration and scale quickly to meet a business case, the majority of applications are rehosted.
  - **Replatforming:** Also known as ???lift, tinker, and shift,??? involves making a few cloud optimizations to realize a tangible benefit. Optimization is achieved without changing the core architecture of the application.
  - **Refactor:** Refactoring (also known as re-architecting) involves reimagining how an application is architected and developed by using cloud-native features. Refactoring is driven by a strong business need to add features, scale, or performance that would otherwise be difficult to achieve in the application???s existing environment.
  - **Repurchase:** Repurchasing involves moving from a traditional license to a software-as-a-service model.
  - **Retain:** Retaining consists of keeping applications that are critical for the business in the source environment. This might include applications that require major refactoring before they can be migrated, or, work that can be postponed until a later time.
  - **Retire:** Retiring is the process of removing applications that are no longer needed.
- **AWS Snow Family:** The AWS Snow Family is a collection of physical devices that help to physically transport up to exabytes of data into and out of AWS.
  - **AWS Snowcone:** AWS Snowcone is a small, rugged, and secure edge computing and data transfer device. It features 2 CPUs, 4 GB of memory, and 8 TB of usable storage.
  - **AWS Snowball Edge:**
    - **Storage Optimized:** Snowball Edge Storage Optimized devices are well suited for large-scale data migrations and recurring transfer workflows, in addition to local computing with higher capacity needs.
    - **Compute Optimized:** Snowball Edge Compute Optimized provides powerful computing resources for use cases such as machine learning, full motion video analysis, analytics, and local computing stacks.
  - **AWS Snowmobile:** AWS Snowmobile is an exabyte-scale data transfer service used to move large amounts of data to AWS. You can transfer up to 100 petabytes of data per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semi trailer truck.
- **Amazon SageMaker:**
- **Amazon Augmented AI (Amazon A2I):**
- **Amazon Lex:**
- **Amazon Textract:**
- **Amazon DeepRacer:**
- **Internet of Things:**
- **AWS Ground Station:**

## Module 10: The Cloud Journey

### [Video: The Cloud Journey](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/lecture/MiAby/introduction-to-module-10)

- **AWS Well-Architected Framework:** The AWS Well-Architected Framework helps you understand how to design and operate reliable, secure, efficient, and cost-effective systems in the AWS Cloud. It provides a way for you to consistently measure your architecture against best practices and design principles and identify areas for improvement. The Well-Architected Framework is based on five pillars:
  - **Operational excellence:** Is the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures. Design principles for operational excellence in the cloud include performing operations as code, annotating documentation, anticipating failure, and frequently making small, reversible changes.
  - **Security:** The Security pillar is the ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies.
  - **Reliability:** Reliability is the ability of a system to do the following:
    - Recover from infrastructure or service disruptions
    - Dynamically acquire computing resources to meet demand
    - Mitigate disruptions such as misconfigurations or transient network issues
      Reliability includes testing recovery procedures, scaling horizontally to increase aggregate system availability, and automatically recovering from failure.
  - **Performance efficiency:** Performance efficiency is the ability to use computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies evolve. Evaluating the performance efficiency of your architecture includes experimenting more often, using serverless architectures, and designing systems to be able to go global in minutes.
  - **Cost optimization:** Cost optimization is the ability to run systems to deliver business value at the lowest price point. Cost optimization includes adopting a consumption model, analyzing and attributing expenditure, and using managed services to reduce the cost of ownership.

## AWS Certified Cloud Practicioner Basics

### [Exam Details](https://www.coursera.org/learn/aws-cloud-practitioner-essentials/supplement/GQ6hE/exam-details)
