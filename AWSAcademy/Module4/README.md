# Cloud Security AWS

## Shared Responsibility Model

- AWS is responsible for the security **OF** the cloud
  - Hardware
  - Software
  - Networking
- Customer is responsible for security **IN** the cloud
    - Customer data
    - Platform, applications, identity and access management
    - Operating system, network and firewall configuration
    - Client-side data encryption and data integrity authentication
    - Server-side encryption of data in transit
    - Network traffic protection

## AWS Security Responsibilities 

- AWS is responsible for the security of the cloud
  - AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services.
- AWS is responsible for the security of customer data

## AWS Client Responsibilities

- Customer is responsible for security in the cloud
  - Customer is responsible for making sure that content they run or store on AWS infrastructure is properly secured
  - Customer is responsible for the security of their AWS account
  - Customer is responsible for the security of their content
  - User access management and identity management are the responsibility of the customer

## Examples of services that AWS manages

- AWS Lambda
- Amazon Relational Database Service (Amazon RDS)
- AWS Elastic Beanstalk

## Examples of services that customers manage

- Amazon Elastic Compute Cloud (Amazon EC2)
- Amazon Elastic Block Store (Amazon EBS)
- Amazon Virtual Private Cloud (Amazon VPC)

## AWS Identity and Access Management (IAM)

- IAM is a web service that helps you securely control access to AWS resources
- You use IAM to control who is authenticated (signed in) and authorized (has permissions) to use resources
- IAM is a feature of your AWS account offered at no additional charge
- You will be charged only for use of other AWS services by your users

-Define IAM users and their access levels
- IAM is universal. It does not apply to regions
- The "root account" is the account created when first setup your AWS account. It has complete Admin access
- New users have no permissions when first created
- Who , to what, and how can they access AWS resources.

## IAM Features

- Person or application is authenticated (signed in) to AWS
- Centralized control of your AWS account
- Shared access to your AWS account
- IAM Groups to group users and apply policies to them
- IAM Policies to define permissions
- IAM Roles to delegate permissions

## Programmatic Access

- Access to AWS CLI, SDK, and other development tools
- Access key ID and secret access key
- Access key ID is used to identify the user
- Secret access key is used to authenticate the user
- Access key ID and secret access key are generated by AWS

## Administration Console Access

- Access to AWS Management Console
- Username and password
- ID or alias (12 digit number or alias)
- MFAs (Multi-Factor Authentication) can be used to add extra security

## IAM Autorization

- IAM policies define permissions 
- All permissions are denied by default and must be explicitly allowed
- If something is not explicitly allowed, it is denied by default

Recommended practice is to use the least privilege principle and give users only the permissions they need to do their job

## IAM Policies

- An IAM policy is a document that defines permissions
- Policies are attached to users, groups, and roles
- Policies are written in JSON (JavaScript Object Notation) format
- Policies define what actions are allowed or denied
two types of policies:
  - Managed policies
  - Inline policies
-Identity-based policies
  - Attached to IAM identities (users, groups, and roles)

-Resource-based policies
    - Attached to resources (S3 buckets, SNS topics, SQS queues, etc.)

- Explicit deny overrides any allow
- Implicit deny denies any request that is not explicitly allowed

## IAM Groups

- A group is a collection of IAM users
- Groups have policies attached to them
- Users inherit the permissions of the group
- Groups cannot be nested
- Groups cannot be used as a permission boundary

## IAM Roles

- A role is an identity that you can create in your AWS account that has specific permissions
- A role is not associated with a specific user or group
- A role is assigned to trusted entities
- A role can be assigned to AWS resources
- A role can be assigned to users in other AWS accounts


## Protection of a new AWS account

- When you first create an AWS account, you begin with a single sign-in identity that has complete access to all AWS services and resources in the account
- This identity is called the AWS **account root** user and is accessed by signing in with the email address and password that you used to create the account
- We strongly recommend that you do not use the root user for your everyday tasks, even the administrative ones
- Instead, adhere to the best practice of using the root user only to create your first IAM user
- Then securely lock away the root user credentials and use them to perform only a few account and service management tasks
- MFAs (Multi-Factor Authentication) can be used to add extra security
- AWS **CloudTrail** can be used to log all actions performed by the root user and all IAM users in the account
- Enable billing alerts to monitor account activity

## AWS Organizations

- AWS Organizations is an account management service that enables you to consolidate multiple AWS accounts into an organization that you create and centrally manage
- Security characteristics of AWS Organizations
  - Account groups called **organizational units (OUs)**
  - Service control policies (SCPs) that centrally control AWS service use across multiple accounts
    - SCPs can be used to restrict access to AWS services
    - Similar to IAM policies, but apply to all accounts in the organization
    - SCPs are applied to OUs
    - SCPs are not applied to the root of the organization
    - SCPs are not applied to individual accounts
    - never grant permissions.
  - IAM integration to apply policies to IAM users and groups
## AWS Key Management Service (KMS)
- AWS Key Management Service (KMS) is a managed service that makes it easy for you to create and control the encryption keys used to encrypt your data.
## Amazon Cognito
- Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily
- Amazon Cognito scales to millions of users and supports sign-in with social identity providers, such as Facebook, Google, and Amazon, and enterprise identity providers via SAML 2.0
## AWS Shield
- AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS
- AWS Shield provides always-on detection and automatic inline mitigations that minimize application downtime and latency
- AWS Shield Standard is available to all AWS customers at no additional cost
- data in transit: data that is moving from one location to another, such as across the internet, or between AWS regions (TLS/SSL , HTTPS)
- data at rest: data that is not moving: stored data

## Working to ensure the compliance of AWS services
- Clients are responsible for the security of their content
- AWS is responsible for the security of the cloud

## AWS Artifact
- AWS Artifact is your go-to, central resource for compliance-related information that matters to you
- It provides on-demand access to AWS’ security and compliance reports and select online agreements