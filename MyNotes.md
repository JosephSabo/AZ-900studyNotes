#  Microsoft Azure Fundamentals: Describe cloud concepts ( MODULE 1)  #

With an on-premises datacenter, you’re responsible for everything. With cloud computing, those responsibilities shift. The shared responsibility model is heavily tied into the cloud service types (covered later in this learning path): infrastructure as a service (IaaS), platform as a service (PaaS), and software as a service (SaaS). IaaS places the most responsibility on the consumer, with the cloud provider being responsible for the basics of physical security, power, and connectivity. On the other end of the spectrum, SaaS places most of the responsibility with the cloud provider. PaaS, being a middle ground between IaaS and SaaS, rests somewhere in the middle and evenly distributes responsibility between the cloud provider and the consumer.

#### You’ll always be responsible for:
- The information and data stored in the cloud
- Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
- The accounts and identities of the people, services, and devices within your organization

#### The cloud provider is always responsible for:
- The physical datacenter
- The physical network
- The physical hosts

#### Your service model will determine responsibility for things like:
- Operating systems
- Network controls
- Applications
- Identity and infrastructure

##### Public cloud:
- No capital expenditures to scale up
- Applications can be quickly provisioned and deprovisioned
- Organizations pay only for what they use
- Organizations don’t have complete control over resources and security

#### private cloud:
- Organizations have complete control over resources and security
- Data is not collocated with other organizations’ data
- Hardware must be purchased for startup and maintenance
- Organizations are responsible for hardware maintenance and updates

#### hybrid cloud:
- Provides the most flexibility
- Organizations determine where to run their applications
- Organizations control security, compliance, or legal requirements

#### Azure Arc
- Azure Arc is a set of technologies that helps manage your cloud environment.
- Azure Arc can help manage your cloud environment, whether it's a public cloud solely on Azure,
a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment
running on multiple cloud providers at once.

#### Azure VMware Solution
What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless 		integration and scalability.

#### Describe the consumption-based model:

When comparing IT infrastructure models, there are two types of expenses to consider. Capital expenditure (CapEx) and operational expenditure (OpEx).
	
- CapEx is typically a one-time, up-front expenditure to purchase or secure tangible resources. A new building, repaving the parking lot, building a datacenter, or buying a company vehicle are examples of CapEx.
- OpEx is spending money on services or products over time. Renting a convention center, leasing a company vehicle, or signing up for cloud services are all examples of OpEx.
- Cloud computing falls under OpEx because cloud computing operates on a consumption-based model. 

This consumption-based model has many benefits, including:
- No upfront costs.
- No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
- The ability to pay for more resources when they're needed.
- The ability to stop paying for resources that are no longer needed.

Additional resources:

	- https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility
 	- https://learn.microsoft.com/en-us/learn/modules/intro-azure-vmware-solution/
  	- https://learn.microsoft.com/en-us/learn/modules/intro-to-azure-hybrid-services/

### Describe the benefits of high availability and scalability in the cloud:


#### High availability:

When you’re deploying an application, a service, or any IT resources, it’s important the resources are available when needed. High availability focuses on ensuring maximum availability, regardless of disruptions or events that may occur.

When you’re architecting your solution, you’ll need to account for service availability guarantees. Azure is a highly available cloud environment with uptime guarantees depending on the service. These guarantees are part of the service-level agreements (SLAs).

#### NOTE: when designing a solution, familiarize yourself with AZURE SLA's, they determine the cost of your solution. ##

#### Scalability:

Another major benefit of cloud computing is the scalability of cloud resources. Scalability refers to the ability to adjust resources to meet demand.

Scaling generally comes in two varieties: vertical and horizontal. Vertical scaling is focused on increasing or decreasing the capabilities of resources. Horizontal scaling is adding or subtracting the number of resources.

#### Vertical scaling

With vertical scaling, if you were developing an app and you needed more processing power, you could vertically scale up to add more CPUs or RAM to the virtual machine. Conversely, if you realized you had over-specified the needs, you could vertically scale down by lowering the CPU or RAM specifications.

#### Horizontal scaling

With horizontal scaling, if you suddenly experienced a steep jump in demand, your deployed resources could be scaled out (either automatically or manually). For example, you could add additional virtual machines or containers, scaling out. In the same manner, if there was a significant drop in demand, deployed resources could be scaled in (either automatically or manually), scaling in.


#### Describe the benefits of reliability and predictability in the cloud

#### Reliability
Reliability is the ability of a system to recover from failures and continue to function. It's also one of the pillars of the Microsoft Azure Well-Architected Framework.

#### Predictability
Predictability can be focused on performance predictability or cost predictability. Both performance and cost predictability are heavily influenced by the Microsoft Azure Well-Architected Framework. Deploy a solution that’s built around this framework and you have a solution whose cost and performance are predictable.

  #### Performance
  - Performance predictability focuses on predicting the resources needed to deliver a positive experience 
 for your customers. Autoscaling, load balancing, and high availability are just some of the cloud 
 concepts that support performance predictability

  #### Cost
  - Cost predictability is focused on predicting or forecasting the cost of the cloud spend. With the cloud, 
 	you can track your resource use in real time, monitor resources to ensure that you’re using them in the 
  	most efficient way, and apply data analytics to find patterns and trends that help better plan resource 
   	deployments. By operating in the cloud and using cloud analytics and information, you can predict future 
    	costs and adjust your resources as needed. You can even use tools like the Total Cost of Ownership (TCO) 
     	or Pricing Calculator to get an estimate of potential cloud spend.

### Describe the benefits of security and governance in the cloud

Whether you’re deploying infrastructure as a service or software as a service, cloud features support governance and compliance. Things like set templates help ensure that all your deployed resources meet corporate standards and government regulatory requirements.

- you can update all your deployed resources to new standards as standards change.
- Cloud-based auditing helps flag any resource that’s out of compliance with your corporate standards and provides mitigation strategies.
- software patches and updates may also automatically be applied, which helps with both governance and security.

On the security side, you can find a cloud solution that matches your security needs.

### Describe the benefits of manageability in the cloud

A major benefit of cloud computing is the manageability options. There are two types of manageability for cloud computing that you’ll learn about in this series, and both are excellent benefits.

  - Management of the cloud speaks to managing your cloud resources. In the cloud, you can:
    - Automatically scale resource deployment based on need.
    - Deploy resources based on a preconfigured template, removing the need for manual configuration.
    - Monitor the health of resources and automatically replace failing resources.
    - Receive automatic alerts based on configured metrics, so you’re aware of performance in real time.

  - Management in the cloud speaks to how you’re able to manage your cloud environment and resources. You can 	manage these:
    - Through a web portal.
    - Using a command line interface.
    - Using APIs.
    - Using PowerShell.

### Describe Infrastructure as a Service (IaaS)

Infrastructure as a service (IaaS) is the most flexible category of cloud services, as it provides you the maximum amount of control for your cloud resources. In an IaaS model, the cloud provider is responsible for maintaining the hardware, network connectivity (to the internet), and physical security. You’re responsible for everything else: operating system installation, configuration, and maintenance; network configuration; database and storage configuration; and so on. With IaaS, you’re essentially renting the hardware in a cloud datacenter, but what you do with that hardware is up to you.

#### Shared responsibility model

IaaS places the largest share of responsibility with you. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet. You’re responsible for installation and configuration, patching and updates, and security.

##### Scenarios

Some common scenarios where IaaS might make sense include:

1) Lift-and-shift migration: You’re standing up cloud resources similar to your on-prem datacenter, and then simply moving the things running on-prem to running on the IaaS infrastructure.

2) Testing and development: You have established configurations for development and test environments that you need to rapidly replicate. You can stand up or shut down the different environments rapidly with an IaaS structure, while maintaining complete control.

### Describe Platform as a Service (PaaS)

Platform as a service (PaaS) is a middle ground between renting space in a datacenter (infrastructure as a service) and paying for a complete and deployed solution (software as a service). In a PaaS environment, the cloud provider maintains the physical infrastructure, physical security, and connection to the internet. They also maintain the operating systems, middleware, development tools, and business intelligence services that make up a cloud solution. In a PaaS scenario, you don't have to worry about the licensing or patching for operating systems and databases.

PaaS is well suited to provide a complete development environment without the headache of maintaining all the development infrastructure.

#### Shared responsibility model


PaaS splits the responsibility between you and the cloud provider. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet, just like in IaaS. In the PaaS model, the cloud provider will also maintain the operating systems, databases, and development tools. Think of PaaS like using a domain joined machine: IT maintains the device with regular updates, patches, and refreshes.

Depending on the configuration, you or the cloud provider may be responsible for networking settings and connectivity within your cloud environment, network and application security, and the directory infrastructure.

#### Scenarios

Some common scenarios where PaaS might make sense include:

1) Development framework: PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.

2) Analytics or business intelligence: Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.

### Describe Software as a Service (SaaS)

Software as a service (SaaS) is the most complete cloud service model from a product perspective. With SaaS, you’re essentially renting or using a fully developed application. Email, financial software, messaging applications, and connectivity software are all common examples of a SaaS implementation.

While the SaaS model may be the least flexible, it’s also the easiest to get up and running. It requires the least amount of technical knowledge or expertise to fully employ.

#### Shared responsibility model

SaaS is the model that places the most responsibility with the cloud provider and the least responsibility with the user. In a SaaS environment you’re responsible for the data that you put into the system, the devices that you allow to connect to the system, and the users that have access. Nearly everything else falls to the cloud provider. The cloud provider is responsible for physical security of the datacenters, power, network connectivity, and application development and patching.

#### Scenarios

Some common scenarios for SaaS are:

-Email and messaging.
-Business productivity applications.
-Finance and expense tracking.


#  Azure Fundamentals: Describe Azure architecture and services (MODULE 2)

## Describe the core architectural components of Azure ##


### What does Azure offer?

#### Be ready for the future:
 
 - Continuous innovation from Microsoft supports your development today and your product visions for 
	tomorrow.
 
#### Build on your terms:
 
- You have choices. With a commitment to open source, and support for all languages and frameworks,
	you can build how you want and deploy where you want.
 
#### Operate hybrid seamlessly:
 
- On-premises, in the cloud, and at the edge, we'll meet you where you are. Integrate and manage your
	environments with tools and services designed for a hybrid cloud solution.
 
#### Trust your cloud:
 
- Get security from the ground up, backed by a team of experts, and proactive compliance trusted by 
	enterprises, governments, and startups.

### Get started with Azure accounts

to startusing Azure you need to open an Azure Account.
Once you have an account, you can create 1 or more subscriptions under that account.

Example: your company can use 1 account for its needs but open several subscriptions and 
use 1 for marketing, one for finance and one for HR. Once you have subscriptions, you can start creating the various resources you need under that subscription.

1) AZURE ACCOUNTANT
2) AZURE SUBSCRIPTION
3) AZURE RESOURCE GROUPS
4) AZURE RESOURCES within the resource groups

### Physical infrastructure ##

In Azure, a physical infrastructure is a datacenter, just like in your companies datacenter.
In Azure, each datacenter is grouped into availability zones or regional zones. so in one zone or region
you can have multiple datacenters, giving the consumer more resiliency and reliability for thier business-critical workloads.

- A region is a geographical area on the planet that contains at least one, but potentially multiple 
	datacenters that are nearby and networked together with a low-latency network.

- Availability zones are physically separate datacenters within an Azure region. Each availability zone is
	 made up of one or more datacenters equipped with independent power, cooling, and networking. An 
	availability zone is set up to be an isolation boundary. If one zone goes down, the other continues 
	working. Availability zones are connected through high-speed, private fiber-optic networks.

### Use availability zones in your apps ##

Availability zones are primarily for VMs, managed disks, load balancers, and SQL databases. Azure services that support availability zones fall into three categories:

- Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).

- Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant 
	storage, SQL Database).

- Non-regional services: Services are always available from Azure geographies and are resilient to zone-
	wide outages as well as region-wide outages.

 ## Region Pairs ##

	Most Azure regions are paired with another region within the same geography (such as US, Europe, or Asia) at least 300 miles away. 
 	This approach allows for the replication of resources across a geography that helps reduce the likelihood of interruptions because 
  	of events such as natural disasters, civil unrest, power outages, or physical network outages that affect an entire region. For example,
   	if a region in a pair was affected by a natural disaster, services would automatically fail over to the other region in its region pair.

		Examples of region pairs in Azure are:

		West US paired with East US

		South-East Asia paired with East Asia.

		Because the pair of regions are directly connected and far enough apart to be isolated from regional disasters, you can use them to provide reliable services and data redundancy.

Additional advantages of region pairs:

	- If an extensive Azure outage occurs, one region out of every pair is prioritized to make sure at least one is restored as quickly as possible for applications hosted in that region pair.
	- Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage.
	- Data continues to reside within the same geography as its pair (except for Brazil South) for tax- and law-enforcement jurisdiction purposes.

## Sovereign Regions ##

Sovereign regions are instances of Azure that are isolated from the main instance of Azure. You may need to use a sovereign region for compliance or legal purposes.

Azure sovereign regions include:

	- US DoD Central, US Gov Virginia, US Gov Iowa and more: These regions are physical and logical network-isolated instances of Azure for U.S. government agencies and partners.
 	  These datacenters are operated by screened U.S. personnel and include additional compliance certifications.
   
	- China East, China North, and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft doesn't directly maintain the datacenters.

# Describe Azure management infrastructure #

The management infrastructure includes Azure resources and resource groups, subscriptions, and accounts.

### Azure resources and resource groups ###

A resource is the basic building block of Azure. Anything you create, provision, deploy, etc. is a resource. Virtual Machines (VMs), virtual networks, databases,
cognitive services, etc. are all considered resources within Azure.

Resource groups are simply groupings of resources. When you create a resource, you’re required to place it into a resource group. While a resource group can contain many resources, a single resource can only be in one resource group at a time.

While a resource group can contain many resources, a single resource can only be in one resource group at a time.

Some resources may be moved between resource groups, but when you move a resource to a new group, it will no longer be associated with the former group.

Additionally, resource groups can't be nested, meaning you can’t put resource group B inside of resource group A.

When you apply an action to a resource group, that action will apply to all the resources within the resource group.

If you delete a resource group, all the resources will be deleted.

If you grant or deny access to a resource group, you’ve granted or denied access to all the resources within the resource group.

## Azure subscriptions ##

subscriptions are a unit of management, billing, and scale. Similar to how resource groups are a way to logically organize resources, 
subscriptions allow you to logically organize your resource groups and facilitate billing.

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/06ab7b75-bfda-4bad-b030-35b56e4b046a)

- Using Azure requires an Azure subscription.
- A subscription provides you with authenticated and authorized access to Azure products and services.
- An Azure subscription links to an Azure account, which is an identity in Azure Active Directory (Azure AD) or in a directory that Azure AD trusts.
- An account can have multiple subscriptions, but it’s only required to have one.
- In a multi-subscription account, you can use the subscriptions to configure different billing models and apply different access-management policies.
### There are two types of subscription boundaries that you can use: ###

### Billing boundary ###

- This subscription type determines how an Azure account is billed for using Azure.
- You can create multiple subscriptions for different types of billing requirements.
- Azure generates separate billing reports and invoices for each subscription so that you can organize and manage costs.

### Access control boundary ###

- Azure applies access-management policies at the subscription level
- you can create separate subscriptions to reflect different organizational structures. An example is that within a business, you have different departments to which you apply distinct Azure subscription policies.
- This billing model allows you to manage and control access to the resources that users provision with specific subscriptions.

## Create additional Azure subscriptions ##

Similar to using resource groups to separate resources by function or access, you might want to create additional subscriptions for resource or billing management purposes.

#### For example, you might choose to create additional subscriptions to separate: ####

#### Environments ####

- You can choose to create subscriptions to set up separate environments for development and testing, security, or to isolate data for compliance reasons.
- This design is particularly useful because resource access control occurs at the subscription level.

#### Organizational structures ####

- You can create subscriptions to reflect different organizational structures. For example, you could limit one team to lower-cost resources, while allowing the IT department a full range.
- This design allows you to manage and control access to the resources that users provision within each subscription.

#### Billing ####

- You can create additional subscriptions for billing purposes.
- Because costs are first aggregated at the subscription level, you might want to create subscriptions to manage and track costs based on your needs.
- For instance, you might want to create one subscription for your production workloads and another subscription for your development and testing workloads.

## Azure management groups ##

- Azure management groups provide a level of scope above subscriptions.
- You organize subscriptions into containers called management groups and apply governance conditions to the management groups
- All subscriptions within a management group automatically inherit the conditions applied to the management group, the same way that resource groups inherit settings from subscriptions and resources inherit from resource groups.
- enterprise-grade management at a large scale, no matter what type of subscriptions you might have.
- Management groups can be nested.

You can build a flexible structure of management groups and subscriptions to organize your resources into a hierarchy for unified policy and access management. The following diagram shows an example of creating a hierarchy for governance by using management groups:

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/9014986e-827d-46eb-9254-c45087661f4c)

Examples of types of Management groups:

- Create a hierarchy that applies a policy. You could limit VM locations to the US West Region in a group called Production. This policy will inherit onto all the subscriptions that are descendants of that management group and will apply to all VMs under those subscriptions. This security policy can't be altered by the resource or subscription owner, which allows for improved governance.
- Provide user access to multiple subscriptions. By moving multiple subscriptions under a management group, you can create one Azure role-based access control (Azure RBAC) assignment on the management group. Assigning Azure RBAC at the management group level means that all sub-management groups, subscriptions, resource groups, and resources underneath that management group would also inherit those permissions. One assignment on the management group can enable users to have access to everything they need instead of scripting Azure RBAC over different subscriptions.

#### Important facts about management groups: 

- 10,000 management groups can be supported in a single directory.
- A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level.
- Each management group and subscription can support only one parent.

## Describe Azure virtual machines

- With Azure Virtual Machines (VMs), you can create and use VMs in the cloud.
- VMs provide infrastructure as a service (IaaS) in the form of a virtualized server and can be used in many ways. Just like a physical computer, you can customize all of the software running on your VM.
- VMs are an ideal choice when you need:
  - Total control over the operating system (OS).
  - The ability to run custom software.
  - To use custom hosting configurations.

### Virtual machine availability sets
Availability sets are designed to ensure that VMs stagger updates and have varied power and network connectivity, preventing you from losing all your VMs with a single network or power failure.

#### Availability sets do this by grouping VMs in two ways: UPDATE DOMAIN and FAULT DOMAIN

- The update domain groups VMs that can be rebooted at the same time. This allows you to apply updates while knowing that only one update domain grouping will be offline at a time. All of the machines in one update domain will be updated. An update group going through the update process is given a 30-minute time to recover before maintenance on the next update domain starts.
- The fault domain groups your VMs by common power source and network switch. By default, an availability set will split your VMs across up to three fault domains. This helps protect against a physical power or networking failure by having VMs in different fault domains (thus being connected to different power and networking resources).

### Examples of when to use VMs

- During testing and development. VMs provide a quick and easy way to create different OS and application configurations. Test and development personnel can then easily delete the VMs when they no longer need them.
- When running applications in the cloud. The ability to run certain applications in the public cloud as opposed to creating a traditional infrastructure to run them can provide substantial economic benefits. For example, an application might need to handle fluctuations in demand. Shutting down VMs when you don't need them or quickly starting them up to meet a sudden increase in demand means you pay only for the resources you use.
- When extending your datacenter to the cloud: An organization can extend the capabilities of its own on-premises network by creating a virtual network in Azure and adding VMs to that virtual network. Applications like SharePoint can then run on an Azure VM instead of running locally. This arrangement makes it easier or less expensive to deploy than in an on-premises environment.
- During disaster recovery: As with running certain types of applications in the cloud and extending an on-premises network to the cloud, you can get significant cost savings by using an IaaS-based approach to disaster recovery. If a primary datacenter fails, you can create VMs running on Azure to run your critical applications and then shut them down when the primary datacenter becomes operational again.

### VM Resources
- Size (purpose, number of processor cores, and amount of RAM)
- Storage disks (hard disk drives, solid state drives, etc.)
- Networking (virtual network, public IP address, and port configuration)

