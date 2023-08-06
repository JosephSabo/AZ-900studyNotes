#######################################################################
## Microsoft Azure Fundamentals: Describe cloud concepts ( MODULE 1) ##
#######################################################################

With an on-premises datacenter, you’re responsible for everything. With cloud computing, those responsibilities shift. The shared responsibility model is heavily tied into the cloud service types (covered later in this learning path): infrastructure as a service (IaaS), platform as a service (PaaS), and software as a service (SaaS). IaaS places the most responsibility on the consumer, with the cloud provider being responsible for the basics of physical security, power, and connectivity. On the other end of the spectrum, SaaS places most of the responsibility with the cloud provider. PaaS, being a middle ground between IaaS and SaaS, rests somewhere in the middle and evenly distributes responsibility between the cloud provider and the consumer.

You’ll always be responsible for:

	The information and data stored in the cloud
	Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
	The accounts and identities of the people, services, and devices within your organization

The cloud provider is always responsible for:

	The physical datacenter
	The physical network
	The physical hosts

Your service model will determine responsibility for things like:

	Operating systems
	Network controls
	Applications
	Identity and infrastructure

Public cloud:
	No capital expenditures to scale up
	Applications can be quickly provisioned and deprovisioned
	Organizations pay only for what they use
	Organizations don’t have complete control over resources and security

private cloud:
	Organizations have complete control over resources and security
	Data is not collocated with other organizations’ data
	Hardware must be purchased for startup and maintenance
	Organizations are responsible for hardware maintenance and updates

hybrid cloud:
	Provides the most flexibility
	Organizations determine where to run their applications
	Organizations control security, compliance, or legal requirements

Azure Arc
	Azure Arc is a set of technologies that helps manage your cloud environment. 
 	Azure Arc can help manage your cloud environment, whether it's a public cloud solely on Azure,
  	a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment
   	running on multiple cloud providers at once.

Azure VMware Solution
	What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless 		integration and scalability.

Describe the consumption-based model:

	When comparing IT infrastructure models, there are two types of expenses to consider. Capital expenditure (CapEx) and operational expenditure (OpEx).
	
 	- CapEx is typically a one-time, up-front expenditure to purchase or secure tangible resources. A new building, repaving the parking lot, building a datacenter, or buying a company vehicle are examples of CapEx.
	
 	- OpEx is spending money on services or products over time. Renting a convention center, leasing a company vehicle, or signing up for cloud services are all examples of OpEx.
	
 	- Cloud computing falls under OpEx because cloud computing operates on a consumption-based model. 

This consumption-based model has many benefits, including:

	No upfront costs.
	No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
	The ability to pay for more resources when they're needed.
	The ability to stop paying for resources that are no longer needed.

Additional resources:
	- https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility
	- https://learn.microsoft.com/en-us/learn/modules/intro-azure-vmware-solution/
	- https://learn.microsoft.com/en-us/learn/modules/intro-to-azure-hybrid-services/
 
===================================================================================
Describe the benefits of high availability and scalability in the cloud:
===================================================================================
High availability:
When you’re deploying an application, a service, or any IT resources, it’s important the resources are available when needed. High availability focuses on ensuring maximum availability, regardless of disruptions or events that may occur.

When you’re architecting your solution, you’ll need to account for service availability guarantees. Azure is a highly available cloud environment with uptime guarantees depending on the service. These guarantees are part of the service-level agreements (SLAs).

NOTE: when designing a solution, familiarize yourself with AZURE SLA's, they determin eht ecost of your solution.
====================================================================================
Scalability:
Another major benefit of cloud computing is the scalability of cloud resources. Scalability refers to the ability to adjust resources to meet demand.

Scaling generally comes in two varieties: vertical and horizontal. Vertical scaling is focused on increasing or decreasing the capabilities of resources. Horizontal scaling is adding or subtracting the number of resources.

Vertical scaling
With vertical scaling, if you were developing an app and you needed more processing power, you could vertically scale up to add more CPUs or RAM to the virtual machine. Conversely, if you realized you had over-specified the needs, you could vertically scale down by lowering the CPU or RAM specifications.

Horizontal scaling
With horizontal scaling, if you suddenly experienced a steep jump in demand, your deployed resources could be scaled out (either automatically or manually). For example, you could add additional virtual machines or containers, scaling out. In the same manner, if there was a significant drop in demand, deployed resources could be scaled in (either automatically or manually), scaling in.
=================================================================================
Describe the benefits of reliability and predictability in the cloud
=================================================================================

Reliability

Reliability is the ability of a system to recover from failures and continue to function. It's also one of the pillars of the Microsoft Azure Well-Architected Framework.

Predictability

Predictability can be focused on performance predictability or cost predictability. Both performance and cost predictability are heavily influenced by the Microsoft Azure Well-Architected Framework. Deploy a solution that’s built around this framework and you have a solution whose cost and performance are predictable.

	Performance
	
	Performance predictability focuses on predicting the resources needed to deliver a positive experience 	for your customers. Autoscaling, load balancing, and high availability are just some of the cloud 	concepts that support performance predictability

	Cost

	Cost predictability is focused on predicting or forecasting the cost of the cloud spend. With the cloud, 	you can track your resource use in real time, monitor resources to ensure that you’re using them in the 	most efficient way, and apply data analytics to find patterns and trends that help better plan resource 	deployments. By operating in the cloud and using cloud analytics and information, you can predict future 	costs and adjust your resources as needed. You can even use tools like the Total Cost of Ownership (TCO) 	or Pricing Calculator to get an estimate of potential cloud spend.

Describe the benefits of security and governance in the cloud
=============================================================

Whether you’re deploying infrastructure as a service or software as a service, cloud features support governance and compliance. Things like set templates help ensure that all your deployed resources meet corporate standards and government regulatory requirements.

- you can update all your deployed resources to new standards as standards change.
- Cloud-based auditing helps flag any resource that’s out of compliance with your corporate standards and provides mitigation strategies.
- software patches and updates may also automatically be applied, which helps with both governance and security.

On the security side, you can find a cloud solution that matches your security needs.

Describe the benefits of manageability in the cloud
===================================================

A major benefit of cloud computing is the manageability options. There are two types of manageability for cloud computing that you’ll learn about in this series, and both are excellent benefits.

	Management of the cloud
	-----------------------

	Management of the cloud speaks to managing your cloud resources. In the cloud, you can:

	-Automatically scale resource deployment based on need.
	-Deploy resources based on a preconfigured template, removing the need for manual configuration.
	-Monitor the health of resources and automatically replace failing resources.
	-Receive automatic alerts based on configured metrics, so you’re aware of performance in real time.

	Management in the cloud
	-----------------------

	Management in the cloud speaks to how you’re able to manage your cloud environment and resources. You can 	manage these:

	-Through a web portal.
	-Using a command line interface.
	-Using APIs.
	-Using PowerShell.

Describe Infrastructure as a Service (IaaS)
===========================================

Infrastructure as a service (IaaS) is the most flexible category of cloud services, as it provides you the maximum amount of control for your cloud resources. In an IaaS model, the cloud provider is responsible for maintaining the hardware, network connectivity (to the internet), and physical security. You’re responsible for everything else: operating system installation, configuration, and maintenance; network configuration; database and storage configuration; and so on. With IaaS, you’re essentially renting the hardware in a cloud datacenter, but what you do with that hardware is up to you.

Shared responsibility model
---------------------------

IaaS places the largest share of responsibility with you. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet. You’re responsible for installation and configuration, patching and updates, and security.

Scenarios
---------
Some common scenarios where IaaS might make sense include:

1) Lift-and-shift migration: You’re standing up cloud resources similar to your on-prem datacenter, and then simply moving the things running on-prem to running on the IaaS infrastructure.

2) Testing and development: You have established configurations for development and test environments that you need to rapidly replicate. You can stand up or shut down the different environments rapidly with an IaaS structure, while maintaining complete control.

Describe Platform as a Service (PaaS)
=====================================

Platform as a service (PaaS) is a middle ground between renting space in a datacenter (infrastructure as a service) and paying for a complete and deployed solution (software as a service). In a PaaS environment, the cloud provider maintains the physical infrastructure, physical security, and connection to the internet. They also maintain the operating systems, middleware, development tools, and business intelligence services that make up a cloud solution. In a PaaS scenario, you don't have to worry about the licensing or patching for operating systems and databases.

PaaS is well suited to provide a complete development environment without the headache of maintaining all the development infrastructure.

Shared responsibility model
---------------------------

PaaS splits the responsibility between you and the cloud provider. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet, just like in IaaS. In the PaaS model, the cloud provider will also maintain the operating systems, databases, and development tools. Think of PaaS like using a domain joined machine: IT maintains the device with regular updates, patches, and refreshes.

Depending on the configuration, you or the cloud provider may be responsible for networking settings and connectivity within your cloud environment, network and application security, and the directory infrastructure.

Scenarios
---------

Some common scenarios where PaaS might make sense include:

1) Development framework: PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.

2) Analytics or business intelligence: Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.

Describe Software as a Service (SaaS)
=====================================

Software as a service (SaaS) is the most complete cloud service model from a product perspective. With SaaS, you’re essentially renting or using a fully developed application. Email, financial software, messaging applications, and connectivity software are all common examples of a SaaS implementation.

While the SaaS model may be the least flexible, it’s also the easiest to get up and running. It requires the least amount of technical knowledge or expertise to fully employ.

Shared responsibility model
---------------------------

SaaS is the model that places the most responsibility with the cloud provider and the least responsibility with the user. In a SaaS environment you’re responsible for the data that you put into the system, the devices that you allow to connect to the system, and the users that have access. Nearly everything else falls to the cloud provider. The cloud provider is responsible for physical security of the datacenters, power, network connectivity, and application development and patching.

Scenarios
---------

Some common scenarios for SaaS are:

-Email and messaging.
-Business productivity applications.
-Finance and expense tracking.


#############################################################################
## Azure Fundamentals: Describe Azure architecture and services (MODULE 2) ##
#############################################################################
