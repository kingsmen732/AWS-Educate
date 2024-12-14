# AWS Questions and Correct Answers

1. **What is cloud computing?**  
   **Correct Answer:** On-demand delivery of IT resources and applications through the internet with pay-as-you-go pricing.

2. **What is another name for on-premises deployment?**  
   **Correct Answer:** Private cloud deployment.

3. **How does the scale of cloud computing help you to save costs?**  
   **Correct Answer:** The aggregated cloud usage from a large number of customers results in lower pay-as-you-go prices.

4. **Which statement is true for the AWS global infrastructure?**  
   **Correct Answer:** A Region consists of two or more Availability Zones.

5. **Which AWS service would you use to grant users permissions?**  
   **Correct Answer:** AWS Identity and Access Management.

6. **What are the five pillars of the AWS Well-Architected Framework?**  
   **Correct Answer:** Operational Excellence, Reliability, Security, Performance Efficiency, Cost Optimization.

7. **Your company has an application that uses Amazon EC2 instances to run the customer-facing website and Amazon RDS database instances to store customers' personal information. How should the developer configure the VPC according to best practices?**  
   **Correct Answer:** Place the Amazon EC2 instances in a public subnet and the Amazon RDS database instances in a private subnet.

8. **Which serverless compute service lets you run functions without provisioning or managing servers?**  
   **Correct Answer:** AWS Lambda.

9. **What are the benefits of cloud computing? (Select TWO.)**  
   **Correct Answers:**  
   - Stop spending money running and maintaining data centers.  
   - Increase speed and agility.

10. **Which option is an example of the customer's responsibility in the AWS shared responsibility model?**  
    **Correct Answer:** Granting user access to Amazon S3.

11. **Which type of EC2 instance would you use if you needed a computing resource that would be in use for at least one full year?**  
    **Correct Answer:** Reserved Instance.

12. **Which statement is true about the AWS 12-month free tier?**  
    **Correct Answer:** The 12-month free trial begins when you set up your AWS account.

13. **Which pillar of the AWS Well-Architected Framework focuses on using computing resources in ways that meet system requirements?**  
    **Correct Answer:** Performance Efficiency.

14. **You want to store data in an object storage service. Which AWS service is best for this type of storage?**  
    **Correct Answer:** Amazon Simple Storage Service (Amazon S3).

15. **Which statement best describes Amazon DynamoDB?**  
    **Correct Answer:** A serverless key-value database service.

# Knowledge Base

Why cloud computing? #cloudcomputing
- IT assets as programmatic resources to quickly set up
  and tear down resources
 - Access resources dynamically for agility 
- flexibility to meet customer needs
- Pay-as-you-go to test and use the system
  without being fully committed

*Definition of cloud computing*
**Cloud computing is the on-demand delivery of IT resources
over the internet with pay-as-you-go pricing.

- On-demand delivery
     On-demand delivery means
     a cloud provider has the
      resources you need, when
      you need them.
- IT resources over the internet
     Servers, networks,
     storage, development
     tools, and applications. 
- Pay-as-you-go pricing
     Pay only for what you
     need when you use it.

**Client-server model**
Modern computing is based on the client-server model.

*A client can be a web
browser or desktop
application that a person
interacts with to make
requests to computer
servers.*

*A server can be services
such as Amazon Elastic
Compute Cloud (Amazon
EC2), a type of virtual
Server*

# Six benefits of cloud computing #benfits-of-cloud 
- Trade upfront expense for
  variable expense
- Stop spending money to run
  and maintain data centers
- Stop guessing capacity
- Benefit from massive
  economies of scale
- Increase speed and agility
- Go global in minutes

# Deployment models include the
following:
• Infrastructure as a service (IaaS)
     Infrastructure as a service (IaaS) contains the basic building blocks for cloud IT. It typically provides access to
    networking features, computers (virtual or on dedicated hardware), and data storage space. Infrastructure as
    service provides the highest level of flexibility and management control over your IT resources.
• Platform as a service (PaaS)
      Platform as a service (PaaS) removes the need for organizations to manage the underlying infrastructure
    (usually hardware and operating systems). They can focus on the deployment and management of
    applications. These tools give developers the ability to be more efficient because they don't need to worry
    about resource procurement, capacity planning, software maintenance, and patching.
• Software as a service (Saas)
    Software as a service (SaaS) is a completed software product that the service provider runs and manages. With
    a SaaS offering, you do not have to think about how the service is maintained or how the underlying
    infrastructure is managed. You only must think about how you will use that particular piece of software.

# Deployment strategies include
the following:
• Cloud
     In a cloud-based deployment model, you can migrate existing applications to the cloud, or you can design and
    build new applications in the cloud. You can build those applications on low-level infrastructure that requires
    your IT staff to manage them. Alternatively, you can build them by using higher-level services that reduce the
    management, architecting, and scaling requirements of the core infrastructure.
• Hybrid
      In a hybrid deployment, cloud-based resources are connected to on-premises infrastructure. You can integrate
     cloud-based resources with legacy IT applications. You might want to use this approach in a number of
    situations. For example, you have legacy applications that are better maintained on premises, or government
    regulations require your business to keep certain records on premises.
• On-premises
	On-premises deployment is also known as a private cloud deployment. In this model, resources are deployed
	on premises by using virtualization and resource management tools. Increase resource utilization by using
	application management and virtualization technologies.

# Planning for failure
- Storage
	 When a file is stored in Amazon S3, the file is
	redundantly copied into every Availability Zone in
	that Region. If one Availability Zone goes down, you
	still have two copies of that file available for you to
	use.
- Compute
	It is a best practice to spread out your computing
	resources across multiple Availability Zones to
	guarantee high availability. So, if one Availability
	Zone goes down, your architecture is still up and
	running.
- Database 
	You can configure your database for Multi-AZ
	deployment. If your Availability Zone with your
	primary database fails, one of the standby
	databases in a healthy Availability Zone
	automatically becomes your new primary database.
	Therefore, your architecture is still functioning.

# AWS Global Infrastructure benefits
- Performance 
- Availability
- Security
- Reliability
- Scalability
- Low Cost

![[Pasted image 20241215032502.png]]
# Billing example
- Amazon EC2
	The service charges in this example include details for the following items:
	• Each Amazon EC2 instance type that has been used
	• The amount of Amazon Elastic Block Storage (Amazon EBS) storage space that has been
	provisioned
	• The length of time that Elastic Load Balancing has been used
	In this example, all the usage amounts are under the thresholds in the AWS Free Tier. Therefore,
	the account owner would not have to pay for any Amazon EC2 usage in this month.
	![[Pasted image 20241215033303.png]]
- Amazon S3
	For Amazon S3 pricing, consider the following cost components:
	• Storage - You pay for only the storage that you use. You are charged the rate to
	store objects in your Amazon S3 buckets. The charges are based on your objects'
	sizes, storage classes, and the amount of time that you stored each object during the
	month.
	• Requests and data retrievals - You pay for requests that were made to your Amazon
	S3 objects and buckets.
	• Data transfer - You pay for data that you transfer into and out of Amazon S3, with a
	few exceptions.
	• Management and replication - You pay for the storage management features that
	you enabled on your account's Amazon SS buckets.
	 ![[Pasted image 20241215033430.png]]
- Aws Lambda
	For AWS Lambda, you are charged based on the number of requests for your
	functions and the time that it takes for them to run.
	With AWS Lambda, you can make 1 million free requests and use up to 3.2
	million seconds of compute time per month.
	You can save on AWS Lambda costs by signing up for a Compute Savings Plan. A
	Compute Savings Plan offers lower compute costs in exchange for committing to
	a consistent amount of usage over a I-year or 3-year term. This plan is an
	example of paying less when you reserve.
	 ![[Pasted image 20241215033523.png]]

# Types of Services
- Managed service
	A managed service is a way to describe the services that require you to manage
	infrastructure management tasks like patching, backup, and repair. These services gran
	you virtual access to the underlying operating system and servers. With managed
	services, you are responsible for scaling and building for high availability.
- Fully managed service
	A fully managed service is a way to describe the services that automate infrastructure
	management tasks that AWS handles, like patching, backup, and repair These services
	do not grant you any virtual access to the underlying operating system or servers. With
	fully managed service, you are still responsible for scaling and building for high
	availability.
- Serverless services
	Serverless is a way to describe the services, practices, and strategies that you can use to
	build more agile applications. In this way, you can innovate and respond to change
	faster. With serverless services, AWS handles infrastructure management tasks like
	capacity provisioning and patching so that you can focus on building applications that
	serve your customers. Serverless services come with automatic scaling, built-in high
	availability, and a pay-for-value billing model.

Example Infrastructure:
![[Pasted image 20241215035406.png]]

# Basic qualification
- Bachelor's degree or equivalent experience
- Experience with systems administration, network administration, IT security, systems architecture or other technical discipline
- Scripting in a cloud-based language such as Python, Java, or
  .NET
- AWS Certifications
