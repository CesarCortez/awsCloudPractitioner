# AWS Cloud Billing and Pricing

## Section 1: AWS Billing and Pricing Overview

There are three main components to AWS billing:

Computing resources :

- charged by the hour or second, depending on the service.
- charged for the time that an instance is running, regardless of whether it is actively being used.
- vary in price depending on the instance type, region, and other factors (linux).

Data transfer :

- charged for data transfer in and out of AWS. In most cases, data transfer between AWS services in the same region is free. Also data transfer inbound to AWS is free (most cases).
- Outbound data transfer is charged per GB, and the price varies depending on the region and the amount of data transferred.

Storage and content delivery :

- charged for the amount of storage used, the number of requests made to the storage service, and the amount of data transferred out of the storage service.

## How to pay for AWS

- Pay as you go
- Pay less when you reserve
- Pay even less per unit by using more : obtain volume discounts as your usage increases
- No contracts or long-term commitments

## Traditional IT vs Cloud IT

Traditional IT :

- Capital expense (CapEx) : money spent to buy or upgrade physical assets such as servers and data centers for your business or organization.
- Upfront investment: you pay for everything up front.
- Long-term commitment
- Capacity planning
- Hardware and software maintenance
- Data center operations

Cloud IT :

- Operational expense (OpEx)
- Pay as you go
- Pay for what you use
- Pay less when you reserve
- No long-term commitment
- No capacity planning
- No hardware or software maintenance
- No data center operations

## AWS Calculator

The AWS Simple Monthly Calculator helps you estimate your monthly AWS bill more efficiently. Using this tool, you can estimate the cost of running your workload in AWS by selecting the region, instance type, storage, and data transfer options that match your use case.

## AWS Free Tier

The AWS Free Tier is designed to give you hands-on experience with a range of AWS services at no charge. For example, you can use the free tier to build and test your application in the cloud, host a website, store and process images, or deliver software or files.

## Consideratios about total cost of ownership (TCO)

- **Server Cost**
  - Hardware: servers, distribution switches, access switches, routers, firewalls, load balancers, etc.
  - Software: Operating system, virtualization, applications, etc.
  - Instalation: power, cooling, racks, etc.
- **Storage Cost**
  - Hardware: storage disk, SAN switches, etc.
  - Software: Storage management, etc.
  - Instalation: power, cooling, racks, etc.
- **Network Cost**
  - Hardware: routers, switches, etc.
  - Software: network management, etc.
  - Instalation: power, cooling, racks, etc.
- **IT Labor Cost**: IT staff, System administrators, Network administrators, etc.

You can save up to 96% if you migrate to AWS.

## AWS Organizations

AWS Organizations is an account management service that enables you to consolidate multiple AWS accounts into an organization that you create and centrally manage. AWS Organizations includes account management and consolidated billing capabilities that enable you to better meet the budgetary, security, and compliance needs of your business.

Multiple accounts can be created under an organization. Each account can be used for a different purpose, such as development, testing, or production. AWS Organizations enables you to manage all of these accounts from a single location.

- IAM : Identity and Access Management

AWS Organizations can be managed using the AWS Management Console, the AWS Command Line Interface (AWS CLI), SDK software development Kits or the AWS Organizations API.

## Section 2: AWS Billing and Pricing Tools

### AWS Billing Dashboard

The AWS Billing and Cost Management Dashboard provides a single location where you can monitor and manage your AWS costs and usage. You can also manage your AWS payment methods and view and download your AWS invoices.

### AWS Cost Explorer

AWS Cost Explorer is a free tool that you can use to view and analyze your AWS costs and usage over time. You can use Cost Explorer to identify trends, pinpoint cost drivers, and detect anomalies in your spend.

### AWS Budgets

AWS Budgets enables you to set custom budgets that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount. You can also use AWS Budgets to set reservation utilization or coverage targets and receive alerts when your utilization drops below the threshold you define.

### AWS Cost and Usage Report

The AWS Cost and Usage Report contains the most comprehensive set of AWS cost and usage data available, including additional metadata about AWS services, pricing, and reservations (e.g., Amazon EC2 Reserved Instances (RIs)). You can use the AWS Cost and Usage Report to track monthly costs and usage, and then create custom reports that analyze cost and usage data for your business.

### AWS Cost Allocation Tags

AWS Cost Allocation Tags enable you to categorize your AWS resources and then track and manage their costs on a detailed level. AWS Cost Allocation Tags can be used to create custom cost allocation reports that break down your AWS costs by the tags you define.

### AWS Bills page

The AWS Bills page provides access to your monthly AWS invoices. You can view your current invoice, as well as your past invoices, and download them as PDF files.

## Section 3: Tecnical Support Plans

### AWS Support Plans

AWS Support Plans provide you with access to tools and expertise that help you succeed with AWS. All AWS customers have access to AWS Basic Support for free. AWS Basic Support provides you with 24x7 access to customer service, documentation, whitepapers, and support forums.
:

- TAM : Technical Account Manager (Proactive Orientation and Guidance, architectural reviews, etc. Only for Business and Enterprise plans )
- AWS Trusted Advisor (Recomended best practices and cost optimization, security, fault tolerance, etc )
- AWS Support API
- AWS Support Concierge (Account Assistance)

### AWS Support Plans

- **Basic** : Free of charge. and offers support for account and billing questions, service limit increases, and other basic service-specific technical support questions.
- **Developer** : Best practices guidance, client-side diagnostic tools, building arquitectures support.
- **Business** : full set of AWS Trusted Advisor checks.
- **Enterprise** : API support, TAM, Concierge support, etc. Technical Account Manager (TAM).

### Severity Levels

- Critical: Production system down, causing severe impact to business operations.

  - Included in Enterprise Support Plan

- Urgent: Production system severely impaired, causing significant impact to business operations.

  - Included in Enterprise and Business Support Plans

- High: Production system impaired, causing moderate impact to business operations.

  - Included in Enterprise and Business Support Plans

- Normal: Production system impaired, causing low impact to business operations.

  - Included in Enterprise, Business, and Developer Support Plans

- Low: General guidance, recommendations, and advice regarding AWS best practices, questions about AWS functionality and features, etc.

  - Included in Enterprise, Business, and Developer Support Plans

BASIC SUPPORT DOES NOT INCLUDE SEVERITY LEVELS (NO TECHNICAL SUPPORT)

# Questions

1. For certains services like Amazon EC2 and Amazon RDS, you can invest in reserved capacity. What options are for reserved instances? (Choose 3 answers)

- [x] AURI (All Upfront Reserved Instance)
- [x] NURI (No Upfront Reserved Instance)
- [x] PURI (Partial Upfront Reserved Instance)
- [ ] MURI
- [ ] DURI 

2. Where can a client go to get billing details abput Amazon Elastic Compute Cloud (Amazon EC2) from 3 months ago ?

- [x] AWS Cost Explorer

3. True or false. To obtain a discount on Amazon EC2 instances, you must pay for the instance for the entire duration of the reservation.

- [x] false

