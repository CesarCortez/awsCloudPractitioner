# Cloud Computing
- Cloud computing is the **on-demand** delivery of compute power.
  - Cloud computing is the **on-demand** delivery of IT resources and applications via the Internet with **pay-as-you-go** pricing.
  - Cloud computing provides a simple way to access servers, storage, databases and a broad set of application services over the Internet.
- With cloud computing you get to <ins>benefit from massive economies of scale</ins>.
- With cloud computing you can <ins>increase your speed and agility</ins>.
- With cloud computing you can <ins>stop guessing capacity</ins>.
- With cloud computing you can <ins>go global in minutes</ins>.
- **Types of cloud computing:**
	- **Infrastructure as a Service** (IaaS): the most basic category of cloud computing services. With IaaS, you rent IT infrastructure—servers and virtual machines (VMs), storage, networks, operating systems—from a cloud provider on a pay-as-you-go basis.
	- **Platform as a Service** (PaaS): refers to cloud computing services that supply an on-demand environment for developing, testing, delivering, and managing software applications. PaaS is designed to make it easier for developers to quickly create web or mobile apps, without worrying about setting up or managing the underlying infrastructure of servers, storage, network, and databases needed for development.
	- **Software as a Service** (SaaS): Refers to end-user applications. With a SaaS offering you do not have to think about how the service is maintained or how the underlying infrastructure is managed; you only need to think about how you will use that particular piece software. A common example of a SaaS application is web-based email where you can send and receive email without having to manage feature additions to the email product or maintaining the servers and operating systems that the email program is running on.
- **Types of cloud implementation:**
	- **Public cloud** (AWS, Azure, GCP): A public cloud is one in which the services and infrastructure are provided off-site over the Internet. These clouds offer the greatest level of efficiency in shared resources; however, they are also more vulnerable than private clouds.
	- **Private cloud** : A private cloud hosting solution, also known as an internal or enterprise cloud, resides on company’s intranet or hosted data center where all of your data is protected behind a firewall. This can be a great option for companies who already have expensive data centers because they can use their current infrastructure. However, private clouds are not as scalable as public clouds.
	- **Hybrid cloud** : A hybrid cloud is a combination of public and private clouds. In a hybrid cloud, an organization provides and manages some resources in-house and has others provided externally. For example, an organization might use a public cloud service, such as Amazon Simple Storage Service (Amazon S3) for archived data but continue to maintain in-house storage for operational customer data.

# AWS Introduction

- Web service: a collection of open protocols and standards used for exchanging data between applications or systems.
- it is not typically tied to any one operating system or programming language.
- AWS: a collection of remote computing services that together make up a cloud computing platform, offered over the Internet by Amazon.com.
- Offers flexible, reliable, scalable, easy-to-use and cost-effective solutions.

# CAF (Cloud Adoption Framework)
- The Cloud Adoption Framework (CAF) provides guidance for adopting the cloud.
- The CAF is designed to help you build a comprehensive approach to cloud computing across your organization, and throughout your IT lifecycle.
- The CAF is divided into six areas of focus, called perspectives.
- The perspectives are:
	- **Business**: The business perspective focuses on the business outcomes that you want to achieve.
	- **People**: The people perspective focuses on the people who are involved in your cloud adoption journey.
	- **Governance**: The governance perspective focuses on the governance model that you will use to manage and measure your cloud adoption journey.
	- **Platform**: The platform perspective focuses on the platform that you will use to support your cloud adoption journey.
	- **Security**: The security perspective focuses on the security controls that you will use to protect your cloud adoption journey.
	- **Operations**: The operations perspective focuses on the operations that you will use to run your cloud adoption journey.

# AWS Categories

- **Compute**: Amazon EC2, AWS Lambda, Amazon ECS, Amazon EKS, AWS Batch, AWS Elastic Beanstalk, AWS Fargate, AWS Serverless Application Repository, AWS Outposts, AWS Wavelength, AWS Snow Family, AWS Thinkbox Deadline
- **Storage**: Amazon S3, Amazon EBS, Amazon EFS, Amazon FSx, Amazon S3 Glacier, AWS Storage Gateway, AWS Snow Family, AWS Backup, AWS DataSync
- **Database**: Amazon RDS, Amazon DynamoDB, Amazon ElastiCache, Amazon Neptune, Amazon QLDB, Amazon DocumentDB (with MongoDB compatibility), Amazon Keyspaces (for Apache Cassandra), Amazon Timestream, Amazon Managed Blockchain, Amazon Redshift, AWS Database Migration Service, AWS Database Migration Service, AWS Datab
- **Migration & Transfer**: AWS Migration Hub, AWS Application Discovery Service, AWS Database Migration Service, AWS Server Migration Service, AWS Snow Family, AWS Transfer Family, AWS DataSync, AWS Application Migration Service, AWS DataSync, AWS Transfer Family, AWS Application Migration Service
- **Networking & Content Delivery**: Amazon VPC, Amazon CloudFront, AWS Direct Connect, Amazon Route 53, AWS Global Accelerator, AWS Transit Gateway, AWS App Mesh, AWS PrivateLink, AWS Network Firewall, AWS Site-to-Site VPN, AWS Client VPN, AWS Global Accelerator, AWS Transit Gateway, AWS App Mesh, AWS PrivateLink, AWS Network Firewall, AWS Site-to-Site VPN, AWS Client VPN
- **Developer Tools**: AWS CodeStar, AWS CodeCommit, AWS CodeBuild, AWS CodeDeploy, AWS CodePipeline, AWS Cloud9, AWS X-Ray, AWS CodeStar, AWS CodeCommit, AWS CodeBuild, AWS CodeDeploy, AWS CodePipeline, AWS Cloud9, AWS X-Ray
- **Management & Governance**: AWS Organizations, AWS CloudFormation, AWS CloudTrail, Amazon CloudWatch, AWS Config, AWS OpsWorks, AWS Service Catalog, AWS Systems Manager, AWS AppConfig, AWS Control Tower, AWS License Manager, AWS Managed Services, AWS Trusted Advisor, AWS Well-Architected Tool, AWS Compute Optimizer, AWS Systems Manager, AWS AppConfig, AWS Control Tower, AWS License Manager, AWS Managed Services, AWS Trusted Advisor, AWS Well-Architected Tool, AWS Compute Optimizer
- **Media Services**: Amazon Kinesis Video Streams, Amazon Interactive Video Service, AWS Elemental MediaConvert, AWS Elemental MediaLive, AWS Elemental MediaPackage, AWS Elemental MediaStore, AWS Elemental MediaTailor, AWS Elemental Appliances & Software, AWS Elemental Link, Amazon Interactive Video Service, AWS Elemental MediaConvert, AWS Elemental MediaLive, AWS Elemental MediaPackage, AWS Elemental MediaStore, AWS Elemental MediaTailor, AWS Elemental Appliances & Software, AWS Elemental Link

- **Machine Learning**: Amazon SageMaker, Amazon Comprehend, Amazon Lex, Amazon Polly, Amazon Rekognition, Amazon Textract, Amazon Forecast, Amazon Personalize, Amazon Augmented AI, Amazon CodeGuru, Amazon Fraud Detector, Amazon Kendra, Amazon Managed Blockchain, Amazon Monitron, Amazon Lookout for Equipment, Amazon Lookout for Vision, Amazon Lookout for Metrics, Amazon Lookout for Vision, Amazon Lookout for Metrics.
- **Analytics**: Amazon Athena, Amazon EMR, Amazon CloudSearch, Amazon Elasticsearch Service, Amazon Kinesis, Amazon Managed Streaming for Apache Kafka (Amazon MSK), Amazon Redshift, Amazon QuickSight, AWS Data Exchange, AWS Data Pipeline, AWS Glue, AWS Lake Formation, AWS Data Exchange, AWS Data Pipeline, AWS Glue, AWS Lake Formation
- **Security, Identity & Compliance**: AWS Identity and Access Management (IAM), Amazon Cloud Directory, Amazon Cognito, AWS Directory Service, AWS Resource Access Manager, AWS Single Sign-On, AWS Key Management Service, AWS Secrets Manager, AWS Certificate Manager, AWS CloudHSM, AWS Firewall Manager, AWS Resource Access Manager, AWS Single Sign-On, AWS Key Management Service, AWS Secrets Manager, AWS Certificate Manager, AWS CloudHSM, AWS Firewall Manager
- **Mobile**: AWS Amplify, Amazon API Gateway, AWS AppSync, Amazon Pinpoint, Amazon SNS, Amazon Cognito, AWS Device Farm, AWS Mobile Hub, AWS Amplify, Amazon API Gateway, AWS AppSync, Amazon Pinpoint, Amazon SNS, Amazon Cognito, AWS Device Farm, AWS Mobile Hub
- **AR & VR**: Amazon Sumerian, Amazon Sumerian
- **Application Integration**: Amazon EventBridge, Amazon MQ, Amazon SNS, Amazon SQS, Amazon AppFlow, Amazon EventBridge, Amazon MQ, Amazon SNS, Amazon SQS, Amazon AppFlow
- **Customer Engagement**: Amazon Connect, Amazon Pinpoint, Amazon Simple Email Service (SES), Amazon Chime, Amazon Connect, Amazon Pinpoint, Amazon Simple Email Service (SES), Amazon Chime
- **Business Applications**: Amazon Honeycode, Amazon Honeycode
- **End User Computing**: Amazon WorkSpaces, Amazon WorkLink, Amazon AppStream 2.0, Amazon WorkDocs, Amazon WorkMail, Amazon WorkSpaces, Amazon WorkLink, Amazon AppStream 2.0, Amazon WorkDocs, Amazon WorkMail
- **Internet of Things**: AWS IoT Core, AWS IoT Greengrass, AWS IoT Analytics, AWS IoT Device Management, AWS IoT Events, AWS IoT SiteWise, AWS IoT Things Graph, AWS IoT Core, AWS IoT Greengrass, AWS IoT Analytics, AWS IoT Device Management, AWS IoT Events, AWS IoT SiteWise, AWS IoT Things Graph

# Six advantages of Amzon Cloud (Benefits)
- **1. Trade capital expense for variable expense:** 
	- No upfront investment
	- Pay for what you use
	- Economies of scale
- **2.Benefit from massive economies of scale:**
	- Lower variable costs than you can get on your own, because usage from hundreds of thousands of customers are aggregated in the cloud.
- **3.Stop guessing about capacity:** 
	- Eliminate guessing on your infrastructure capacity needs. 
	- When you make a capacity decision prior to deploying an application, you often either end up sitting on expensive idle resources or dealing with limited capacity. 
	- You can access as much or as little as you need, and scale up and down as required with only a few minutes notice.
- **4.Increase speed and agility:**
	- In a cloud computing environment, new IT resources are only ever a click away, which means you reduce the time to make those resources available to your developers from weeks to just minutes. 
- **5.Stop spending money running and maintaining data centres:**
	- Focus on projects that differentiate your business, not the infrastructure. 
	- Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking and powering servers.
- **6.Go global in minutes:**
	- Easily deploy your application in multiple regions around the world with just a few clicks. 
	- This means you can provide a lower latency and better experience for your customers at minimal cost.