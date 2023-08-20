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

### Azure management groups ##

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

### Describe Azure virtual machines

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

### Describe Azure Containers

- Containers are a virtualization environment.
- Much like running multiple virtual machines on a single physical host, you can run multiple containers on a single physical or virtual host.
- Unlike virtual machines, you don't manage the operating system for a container.
- Containers are lightweight and designed to be created, scaled out, and stopped dynamically.
- It's possible to create and deploy virtual machines as application demand increases, but containers are a lighter weight, more agile method.
- Containers are designed to allow you to respond to changes on demand.
- With containers, you can quickly restart if there's a crash or hardware interruption.
- One of the most popular container engines is Docker, and Azure supports Docker.

#### Azure Container Instances
- Azure Container Instances offer the fastest and simplest way to run a container in Azure; without having to manage any virtual machines or adopt any additional services.
- Azure Container Instances are a platform as a service (PaaS) offering.
- Azure Container Instances allow you to upload your containers and then the service will run the containers for you.

#### Azure Container Apps
- Azure Container Apps are similar in many ways to a container instance.
- They allow you to get up and running right away, they remove the container management piece, and they're a PaaS offering.
- Container Apps have extra benefits such as the ability to incorporate load balancing and scaling.

#### Azure Kubernetes Service
- Azure Kubernetes Service (AKS) is a container orchestration service.
- An orchestration service manages the lifecycle of containers.
- When you're deploying a fleet of containers, AKS can make fleet management simpler and more efficient.

#### Use containers in your solutions
- Containers are often used to create solutions by using a microservice architecture. This architecture is where you break solutions into smaller, independent pieces. For example, you might split a website into a container hosting your front end, another hosting your back end, and a third for storage. This split allows you to separate portions of your app into logical sections that can be maintained, scaled, or updated independently.
- Imagine your website back-end has reached capacity but the front end and storage aren't being stressed. With containers, you could scale the back end separately to improve performance. If something necessitated such a change, you could also choose to change the storage service or modify the front end without impacting any of the other components.

### Describe Azure Functions
- Azure Functions is an event-driven, serverless compute option that doesn’t require maintaining virtual machines or containers.
- If you build an app using VMs or containers, those resources have to be “running” in order for your app to function.
- With Azure Functions, an event wakes the function, alleviating the need to keep resources provisioned when there are no events.

#### Benefits of Azure Functions
- Using Azure Functions is ideal when you're only concerned about the code running your service and not about the underlying platform or infrastructure. Functions are commonly used when you need to perform work in response to an event (often via a REST request), timer, or message from another Azure service, and when that work can be completed quickly, within seconds or less.
- Functions scale automatically based on demand, so they may be a good choice when demand is variable.
- Azure Functions runs your code when it's triggered and automatically deallocates resources when the function is finished. In this model, you're only charged for the CPU time used while your function runs.
- Functions can be either stateless or stateful. When they're stateless (the default), they behave as if they're restarted every time they respond to an event. When they're stateful (called Durable Functions), a context is passed through the function to track prior activity.
- Functions are a key component of serverless computing. They're also a general compute platform for running any type of code. If the needs of the developer's app change, you can deploy the project in an environment that isn't serverless. This flexibility allows you to manage scaling, run on virtual networks, and even completely isolate the functions.

### Describe application hosting options

#### Azure App Service
- pp Service enables you to build and host web apps, background jobs, mobile back-ends, and RESTful APIs in the programming language of your choice without managing infrastructure.
- It offers automatic scaling and high availability.
- App Service supports Windows and Linux.
- It enables automated deployments from GitHub, Azure DevOps, or any Git repo to support a continuous deployment model.
- Azure App Service is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends.
- It supports multiple languages, including .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python.
- It also supports both Windows and Linux environments.

#### Types of app services
- With App Service, you can host most common app service styles like:
  - Web apps
  - API apps
  - WebJobs
  - Mobile apps
- App Service handles most of the infrastructure decisions you deal with in hosting web-accessible apps:
  - Deployment and management are integrated into the platform.
  - Endpoints can be secured.
  - Sites can be scaled quickly to handle high traffic loads.
  - The built-in load balancing and traffic manager provide high availability.

#### Web apps
- App Service includes full support for hosting web apps by using ASP.NET, ASP.NET Core, Java, Ruby, Node.js, PHP, or Python. You can choose either Windows or Linux as the host operating system.

#### API apps
- Much like hosting a website, you can build REST-based web APIs by using your choice of language and framework.
- You get full Swagger support and the ability to package and publish your API in Azure Marketplace.
- The produced apps can be consumed from any HTTP- or HTTPS-based client.

#### WebJobs
- You can use the WebJobs feature to run a program (.exe, Java, PHP, Python, or Node.js) or script (.cmd, .bat, PowerShell, or Bash) in the same context as a web app, API app, or mobile app.
- They can be scheduled or run by a trigger.
- WebJobs are often used to run background tasks as part of your application logic.

#### Mobile apps
- Use the Mobile Apps feature of App Service to quickly build a back end for iOS and Android apps. With just a few actions in the Azure portal, you can:
  - Store mobile app data in a cloud-based SQL database
  - Authenticate customers against common social providers, such as MSA, Google, Twitter, and Facebook.
  - Send push notifications.
  - Execute custom back-end logic in C# or Node.js.
- On the mobile app side, there's SDK support for native iOS and Android, Xamarin, and React native apps.

### Describe Azure Virtual Networking
- Azure virtual networks and virtual subnets enable Azure resources, such as VMs, web apps, and databases, to communicate with each other, with users on the internet, and with your on-premises client computers. You can think of an Azure network as an extension of your on-premises network with resources that link other Azure resources.
- Azure virtual networks provide the following key networking capabilities:
  - Isolation and segmentation
  - Internet communications
  - Communicate between Azure resources
  - Communicate with on-premises resources
  - Route network traffic
  - Filter network traffic
  - Connect virtual networks

- Azure virtual networking supports both public and private endpoints to enable communication between external or internal resources with other internal resources.
  - Public endpoints have a public IP address and can be accessed from anywhere in the world.
  - Private endpoints exist within a virtual network and have a private IP address from within the address space of that virtual network.

#### Isolation and segmentation
- Azure virtual network allows you to create multiple isolated virtual networks.
- When you set up a virtual network, you define a private IP address space by using either public or private IP address ranges.
- The IP range only exists within the virtual network and isn't internet routable.
- You can divide that IP address space into subnets and allocate part of the defined address space to each named subnet.
- For name resolution, you can use the name resolution service that's built into Azure.
- You also can configure the virtual network to use either an internal or an external DNS server.

#### Internet communications
- You can enable incoming connections from the internet by assigning a public IP address to an Azure resource, or putting the resource behind a public load balancer.

#### Communicate between Azure resources
- You'll want to enable Azure resources to communicate securely with each other. You can do that in one of two ways:
  - Virtual networks can connect not only VMs but other Azure resources, such as the App Service Environment for Power Apps, Azure Kubernetes Service, and Azure virtual machine scale sets.
  - Service endpoints can connect to other Azure resource types, such as Azure SQL databases and storage accounts. This approach enables you to link multiple Azure resources to virtual networks to improve security and provide optimal routing between resources.

#### Communicate with on-premises resources
- Azure virtual networks enable you to link resources together in your on-premises environment and within your Azure subscription.
- There are three mechanisms for you to achieve this connectivity:
  - Point-to-site virtual private network connections are from a computer outside your organization back into your corporate network. In this case, the client computer initiates an encrypted VPN connection to connect to the Azure virtual network.
  - Site-to-site virtual private networks link your on-premises VPN device or gateway to the Azure VPN gateway in a virtual network. In effect, the devices in Azure can appear as being on the local network. The connection is encrypted and works over the internet.
  - Azure ExpressRoute provides a dedicated private connectivity to Azure that doesn't travel over the internet. ExpressRoute is useful for environments where you need greater bandwidth and even higher levels of security.

#### Route network traffic
- By default, Azure routes traffic between subnets on any connected virtual networks, on-premises networks, and the internet.
- You also can control routing and override those settings, as follows:
  - Route tables allow you to define rules about how traffic should be directed. You can create custom route tables that control how packets are routed between subnets.
  - Border Gateway Protocol (BGP) works with Azure VPN gateways, Azure Route Server, or Azure ExpressRoute to propagate on-premises BGP routes to Azure virtual networks.

#### Filter network traffic
- Azure virtual networks enable you to filter traffic between subnets by using the following approaches:
  - Network security groups are Azure resources that can contain multiple inbound and outbound security rules. You can define these rules to allow or block traffic, based on factors such as source and destination IP address, port, and protocol.
  - Network virtual appliances are specialized VMs that can be compared to a hardened network appliance. A network virtual appliance carries out a particular network function, such as running a firewall or performing wide area network (WAN) optimization.

#### Connect virtual networks
- You can link virtual networks together by using virtual network peering.
- Peering allows two virtual networks to connect directly to each other.
- Network traffic between peered networks is private, and travels on the Microsoft backbone network, never entering the public internet.
- Peering enables resources in each virtual network to communicate with each other.
- These virtual networks can be in separate regions, which allows you to create a global interconnected network through Azure.
- User-defined routes (UDR) allow you to control the routing tables between subnets within a virtual network or between virtual networks. This allows for greater control over network traffic flow.

### Describe Azure Virtual Private Networks
- A virtual private network (VPN) uses an encrypted tunnel within another network.
- VPNs are typically deployed to connect two or more trusted private networks to one another over an untrusted network (typically the public internet).
- Traffic is encrypted while traveling over the untrusted network to prevent eavesdropping or other attacks.
- VPNs can enable networks to safely and securely share sensitive information.

#### VPN gateways
- A VPN gateway is a type of virtual network gateway. Azure VPN Gateway instances are deployed in a dedicated subnet of the virtual network and enable the following connectivity:
  - Connect on-premises datacenters to virtual networks through a site-to-site connections
  - Connect individual devices to virtual networks through a point-to-site connection.
  - Connect virtual networks to other virtual networks through a network-to-network connection.

- All data transfer is encrypted inside a private tunnel as it crosses the internet.
- You can deploy only one VPN gateway in each virtual network. However, you can use one gateway to connect to multiple locations, which includes other virtual networks or on-premises datacenters.

- When setting up a VPN gateway, you must specify the type of VPN:
  - Policy Based
  - Route Based
- The primary distinction between these two types is how they determine which traffic needs encryption.
- In Azure, regardless of the VPN type, the method of authentication employed is a pre-shared key.

  - Policy-based VPN gateways specify statically the IP address of packets that should be encrypted through each tunnel. This type of device evaluates every data packet against those sets of IP addresses to choose the tunnel where that packet is going to be sent through.
  - In Route-based gateways, IPSec tunnels are modeled as a network interface or virtual tunnel interface. IP routing (either static routes or dynamic routing protocols) decides which one of these tunnel interfaces to use when sending each packet. Route-based VPNs are the preferred connection method for on-premises devices. They're more resilient to topology changes such as the creation of new subnets.

- Use a route-based VPN gateway if you need any of the following types of connectivity:
  - Connections between virtual networks
  - Point-to-site connections
  - Multisite connections
  - Coexistence with an Azure ExpressRoute gateway

#### High-availability scenarios
- If you’re configuring a VPN to keep your information safe, you also want to be sure that it’s a highly available and fault tolerant VPN configuration. There are a few ways to maximize the resiliency of your VPN gateway.

##### Active/standby
- By default, VPN gateways are deployed as two instances in an active/standby configuration, even if you only see one VPN gateway resource in Azure. When planned maintenance or unplanned disruption affects the active instance, the standby instance automatically assumes responsibility for connections without any user intervention. Connections are interrupted during this failover, but they're typically restored within a few seconds for planned maintenance and within 90 seconds for unplanned disruptions.
##### Active/active
- With the introduction of support for the BGP routing protocol, you can also deploy VPN gateways in an active/active configuration. In this configuration, you assign a unique public IP address to each instance. You then create separate tunnels from the on-premises device to each IP address. You can extend the high availability by deploying an additional VPN device on-premises.
##### ExpressRoute failover
- Another high-availability option is to configure a VPN gateway as a secure failover path for ExpressRoute connections. ExpressRoute circuits have resiliency built in. However, they aren't immune to physical problems that affect the cables delivering connectivity or outages that affect the complete ExpressRoute location. In high-availability scenarios, where there's risk associated with an outage of an ExpressRoute circuit, you can also provision a VPN gateway that uses the internet as an alternative method of connectivity. In this way, you can ensure there's always a connection to the virtual networks.
##### Zone-redundant gateways
- In regions that support availability zones, VPN gateways and ExpressRoute gateways can be deployed in a zone-redundant configuration. This configuration brings resiliency, scalability, and higher availability to virtual network gateways. Deploying gateways in Azure availability zones physically and logically separates gateways within a region while protecting your on-premises network connectivity to Azure from zone-level failures. These gateways require different gateway stock keeping units (SKUs) and use Standard public IP addresses instead of Basic public IP addresses.

### Describe Azure ExpressRoute

- Azure ExpressRoute lets you extend your on-premises networks into the Microsoft cloud over a private connection, with the help of a connectivity provider.
- This connection is called an ExpressRoute Circuit.
- With ExpressRoute, you can establish connections to Microsoft cloud services, such as Microsoft Azure and Microsoft 365. This allows you to connect offices, datacenters, or other facilities to the Microsoft cloud.
- Each location would have its own ExpressRoute circuit.

#### Features and benefits of ExpressRoute
- There are several benefits to using ExpressRoute as the connection service between Azure and on-premises networks.

  - Connectivity to Microsoft cloud services across all regions in the geopolitical region.
  - Global connectivity to Microsoft services across all regions with the ExpressRoute Global Reach.
  - Dynamic routing between your network and Microsoft via Border Gateway Protocol (BGP).
  - Built-in redundancy in every peering location for higher reliability.

#### Connectivity to Microsoft cloud services
- ExpressRoute enables direct access to the following services in all regions:

  - Microsoft Office 365
  - Microsoft Dynamics 365
  - Azure compute services, such as Azure Virtual Machines
  - Azure cloud services, such as Azure Cosmos DB and Azure Storage

#### Global connectivity
- You can enable ExpressRoute Global Reach to exchange data across your on-premises sites by connecting your ExpressRoute circuits. For example, say you had an office in Asia and a datacenter in Europe, both with ExpressRoute circuits connecting them to the Microsoft network. You could use ExpressRoute Global Reach to connect those two facilities, allowing them to communicate without transferring data over the public internet.

#### Dynamic routing
- ExpressRoute uses the BGP. BGP is used to exchange routes between on-premises networks and resources running in Azure. This protocol enables dynamic routing between your on-premises network and services running in the Microsoft cloud.

#### Built-in redundancy
- Each connectivity provider uses redundant devices to ensure that connections established with Microsoft are highly available. You can configure multiple circuits to complement this feature.

#### ExpressRoute connectivity models
- ExpressRoute supports four models that you can use to connect your on-premises network to the Microsoft cloud:

  - CloudExchange colocation
  - Point-to-point Ethernet connection
  - Any-to-any connection
  - Directly from ExpressRoute sites

#### Co-location at a cloud exchange
- Co-location refers to your datacenter, office, or other facility being physically co-located at a cloud exchange, such as an ISP. If your facility is co-located at a cloud exchange, you can request a virtual cross-connect to the Microsoft cloud.

#### Point-to-point Ethernet connection
- Point-to-point ethernet connection refers to using a point-to-point connection to connect your facility to the Microsoft cloud.

#### Any-to-any networks
- With any-to-any connectivity, you can integrate your wide area network (WAN) with Azure by providing connections to your offices and datacenters. Azure integrates with your WAN connection to provide a connection like you would have between your datacenter and any branch offices.

#### Directly from ExpressRoute sites
- You can connect directly into the Microsoft's global network at a peering location strategically distributed across the world. ExpressRoute Direct provides dual 100 Gbps or 10-Gbps connectivity, which supports Active/Active connectivity at scale.

#### Security considerations
- With ExpressRoute, your data doesn't travel over the public internet, so it's not exposed to the potential risks associated with internet communications. ExpressRoute is a private connection from your on-premises infrastructure to your Azure infrastructure. Even if you have an ExpressRoute connection, DNS queries, certificate revocation list checking, and Azure Content Delivery Network requests are still sent over the public internet.

### Describe Azure DNS
- Azure DNS is a hosting service for DNS domains that provides name resolution by using Microsoft Azure infrastructure.
- By hosting your domains in Azure, you can manage your DNS records using the same credentials, APIs, tools, and billing as your other Azure services.

#### Benefits of Azure DNS
- Azure DNS leverages the scope and scale of Microsoft Azure to provide numerous benefits, including:

  - Reliability and performance
  - Security
  - Ease of Use
  - Customizable virtual networks
  - Alias records

#### Reliability and performance
- DNS domains in Azure DNS are hosted on Azure's global network of DNS name servers, providing resiliency and high availability.
- Azure DNS uses anycast networking, so each DNS query is answered by the closest available DNS server to provide fast performance and high availability for your domain.

#### Security
Azure DNS is based on Azure Resource Manager, which provides features such as:

  - Azure role-based access control (Azure RBAC) to control who has access to specific actions for your organization.
  - Activity logs to monitor how a user in your organization modified a resource or to find an error when troubleshooting.
  - Resource locking to lock a subscription, resource group, or resource. Locking prevents other users in your organization from accidentally deleting or modifying critical resources.

#### Ease of use
Azure DNS can manage DNS records for your Azure services and provide DNS for your external resources as well. Azure DNS is integrated in the Azure portal and uses the same credentials, support contract, and billing as your other Azure services.

Because Azure DNS is running on Azure, it means you can manage your domains and records with the Azure portal, Azure PowerShell cmdlets, and the cross-platform Azure CLI. Applications that require automated DNS management can integrate with the service by using the REST API and SDKs.

#### Customizable virtual networks with private domains
Azure DNS also supports private DNS domains. This feature allows you to use your own custom domain names in your private virtual networks, rather than being stuck with the Azure-provided names.

#### Alias records
- Azure DNS also supports alias record sets. You can use an alias record set to refer to an Azure resource, such as an Azure public IP address, an Azure Traffic Manager profile, or an Azure Content Delivery Network (CDN) endpoint.
- If the IP address of the underlying resource changes, the alias record set seamlessly updates itself during DNS resolution.
- The alias record set points to the service instance, and the service instance is associated with an IP address.

## Describe Azure storage services

### Describe Azure storage accounts
A storage account provides a unique namespace for your Azure Storage data that's accessible from anywhere in the world over HTTP or HTTPS. Data in this account is secure, highly available, durable, and massively scalable.

- When you create your storage account, you’ll start by picking the storage account type.
- The type of account determines the storage services and redundancy options and has an impact on the use cases.
- Below is a list of redundancy options that will be covered later in this module:

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/e6e8494d-4952-4990-8a26-2e87cbccb82c)

#### Storage account endpoints
One of the benefits of using an Azure Storage Account is having a unique namespace in Azure for your data. In order to do this, every storage account in Azure must have a unique-in-Azure account name. The combination of the account name and the Azure Storage service endpoint forms the endpoints for your storage account.

When naming your storage account, keep these rules in mind:
- Storage account names must be between 3 and 24 characters in length and may contain numbers and lowercase letters only.
- Your storage account name must be unique within Azure. No two storage accounts can have the same name. This supports the ability to have a unique, accessible namespace in Azure.

The following table shows the endpoint format for Azure Storage services:

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/c0035a70-f3b0-47ab-b470-63d734013a84)

### Describe Azure storage redundancy
Azure Storage always stores multiple copies of your data so that it's protected from planned and unplanned events such as transient hardware failures, network or power outages, and natural disasters. Redundancy ensures that your storage account meets its availability and durability targets even in the face of failures.

When deciding which redundancy option is best for your scenario, consider the tradeoffs between lower costs and higher availability. The factors that help determine which redundancy option you should choose include:

- How your data is replicated in the primary region.
- Whether your data is replicated to a second region that is geographically distant to the primary region, to protect against regional disasters.
- Whether your application requires read access to the replicated data in the secondary region if the primary region becomes unavailable.

#### Redundancy in the primary region
Data in an Azure Storage account is always replicated three times in the primary region. 
Azure Storage offers two options for how your data is replicated in the primary region:
- locally redundant storage (LRS)
- zone-redundant storage (ZRS).

##### Locally redundant storage

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/b8c19205-afdf-4964-b689-13890731be84)

- Locally redundant storage (LRS) replicates your data three times within a single data center in the primary region.
- LRS provides at least 11 nines of durability (99.999999999%) of objects over a given year.
- LRS is the lowest-cost redundancy option and offers the least durability compared to other options.
- LRS protects your data against server rack and drive failures.
##### (However, if a disaster such as fire or flooding occurs within the data center, all replicas of a storage account using LRS may be lost or unrecoverable. To mitigate this risk, Microsoft recommends using zone-redundant storage (ZRS), geo-redundant storage (GRS), or geo-zone-redundant storage (GZRS).)

##### Zone-redundant storage

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/3ad2d2e7-fdc5-4052-aef7-db7c5797047a)

- For Availability Zone-enabled Regions, zone-redundant storage (ZRS) replicates your Azure Storage data synchronously across three Azure availability zones in the primary region.
- ZRS offers durability for Azure Storage data objects of at least 12 nines (99.9999999999%) over a given year.
- With ZRS, your data is still accessible for both read and write operations even if a zone becomes unavailable.
- No remounting of Azure file shares from the connected clients is required.
- If a zone becomes unavailable, Azure undertakes networking updates, such as DNS repointing.
- These updates may affect your application if you access data before the updates have completed.
- ##### Microsoft recommends using ZRS in the primary region for scenarios that require high availability. ZRS is also recommended for restricting replication of data within a country or region to meet data governance requirements.

#### Redundancy in a secondary region
- For applications requiring high durability, you can choose to additionally copy the data in your storage account to a secondary region that is hundreds of miles away from the primary region. If the data in your storage account is copied to a secondary region, then your data is durable even in the event of a catastrophic failure that prevents the data in the primary region from being recovered.

- When you create a storage account, you select the primary region for the account. The paired secondary region is based on Azure Region Pairs, and can't be changed.

- Azure Storage offers two options for copying your data to a secondary region: geo-redundant storage (GRS) and geo-zone-redundant storage (GZRS). GRS is similar to running LRS in two regions, and GZRS is similar to running ZRS in the primary region and LRS in the secondary region.

- By default, data in the secondary region isn't available for read or write access unless there's a failover to the secondary region. If the primary region becomes unavailable, you can choose to fail over to the secondary region. After the failover has completed, the secondary region becomes the primary region, and you can again read and write data.

##### Geo-redundant storage

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/dbedd79d-a979-4701-b4d8-00c6c6310171)

- GRS copies your data synchronously three times within a single physical location in the primary region using LRS.
- It then copies your data asynchronously to a single physical location in the secondary region (the region pair) using LRS.
- GRS offers durability for Azure Storage data objects of at least 16 nines (99.99999999999999%) over a given year.

##### Geo-zone-redundant storage

![image](https://github.com/JosephSabo/AZ-900studyNotes/assets/47758130/e6095f36-36b1-47d2-9b9e-11fe14ca2c80)

- GZRS combines the high availability provided by redundancy across availability zones with protection from regional outages provided by geo-replication.
- Data in a GZRS storage account is copied across three Azure availability zones in the primary region (similar to ZRS) and is also replicated to a secondary geographic region, using LRS, for protection from regional disasters.
- Microsoft recommends using GZRS for applications requiring maximum consistency, durability, and availability, excellent performance, and resilience for disaster recovery.
- GZRS is designed to provide at least 16 nines (99.99999999999999%) of durability of objects over a given year.

### Describe Azure storage services
The Azure Storage platform includes the following data services:

- Azure Blobs: A massively scalable object store for text and binary data. Also includes support for big data analytics through Data Lake Storage Gen2.
- Azure Files: Managed file shares for cloud or on-premises deployments.
- Azure Queues: A messaging store for reliable messaging between application components.
- Azure Disks: Block-level storage volumes for Azure VMs.
- Azure Tables: NoSQL table option for structured, non-relational data.

#### Benefits of Azure Storage

- Durable and highly available. Redundancy ensures that your data is safe if transient hardware failures occur. You can also opt to replicate data across data centers or geographical regions for additional protection from local catastrophes or natural disasters. Data replicated in this way remains highly available if an unexpected outage occurs.
- Secure. All data written to an Azure storage account is encrypted by the service. Azure Storage provides you with fine-grained control over who has access to your data.
- Scalable. Azure Storage is designed to be massively scalable to meet the data storage and performance needs of today's applications.
- Managed. Azure handles hardware maintenance, updates, and critical issues for you.
- Accessible. Data in Azure Storage is accessible from anywhere in the world over HTTP or HTTPS. Microsoft provides client libraries for Azure Storage in a variety of languages, including .NET, Java, Node.js, Python, PHP, Ruby, Go, and others, as well as a mature REST API. Azure Storage supports scripting in Azure PowerShell or Azure CLI. And the Azure portal and Azure Storage Explorer offer easy visual solutions for working with your data.

#### Azure Blobs

- object storage solution
- can store data such as text or binary
- its unstructured
- can manage thousands of siultaneous uploads
- massive amounts if video data
- constantly growing log files
- are not limited to common file formats
- data is uploaded as blobs, and Azure takes care of the physical storage needs
- Blob storage is ideal for:

  - Serving images or documents directly to a browser.
  - Storing files for distributed access.
  - Streaming video and audio.
  - Storing data for backup and restore, disaster recovery, and archiving.
  - Storing data for analysis by an on-premises or Azure-hosted service.

##### Accessing blob storage

Objects in blob storage can be accessed from anywhere in the world via HTTP or HTTPS. Users or client applications can access blobs via URLs, the Azure Storage REST API, Azure PowerShell, Azure CLI, or an Azure Storage client library. The storage client libraries are available for multiple languages, including .NET, Java, Node.js, Python, PHP, and Ruby.

##### Blob storage tiers

- Azure Storage offers different access tiers for your blob storage, helping you store object data in the most cost-effective manner. The available access tiers include:

  - Hot access tier: Optimized for storing data that is accessed frequently (for example, images for your website).
  - Cool access tier: Optimized for data that is infrequently accessed and stored for at least 30 days (for example, invoices for your customers).
  - Cold access tier: Optimized for storing data that is infrequently accessed and stored for at least 90 days.
  - Archive access tier: Appropriate for data that is rarely accessed and stored for at least 180 days, with flexible latency requirements (for example, long-term backups).

- The following considerations apply to the different access tiers:

  - Hot, cool, and cold access tiers can be set at the account level. The archive access tier isn't available at the account level.
  - Hot, cool, cold, and archive tiers can be set at the blob level, during or after upload.
  - Data in the cool and cold access tiers can tolerate slightly lower availability, but still requires high durability, retrieval latency, and throughput characteristics similar to hot data. For cool and cold data, a lower availability service-level agreement (SLA) and higher access costs compared to hot data are acceptable trade-offs for lower storage costs.
  - Archive storage stores data offline and offers the lowest storage costs, but also the highest costs to rehydrate and access data.

#### Azure Files

- Azure File storage offers fully managed file shares in the cloud that are accessible via the industry standard Server Message Block (SMB) or Network File System (NFS) protocols.
- Azure Files file shares can be mounted concurrently by cloud or on-premises deployments.
- SMB Azure file shares are accessible from Windows, Linux, and macOS clients.
- NFS Azure Files shares are accessible from Linux or macOS clients.
- Additionally, SMB Azure file shares can be cached on Windows Servers with Azure File Sync for fast access near where the data is being used.

##### Azure Files key benefits:
- Shared access: Azure file shares support the industry standard SMB and NFS protocols, meaning you can seamlessly replace your on-premises file shares with Azure file shares without worrying about application compatibility.
- Fully managed: Azure file shares can be created without the need to manage hardware or an OS. This means you don't have to deal with patching the server OS with critical security upgrades or replacing faulty hard disks.
- Scripting and tooling: PowerShell cmdlets and Azure CLI can be used to create, mount, and manage Azure file shares as part of the administration of Azure applications. You can create and manage Azure file shares using Azure portal and Azure Storage Explorer.
- Resiliency: Azure Files has been built from the ground up to always be available. Replacing on-premises file shares with Azure Files means you don't have to wake up in the middle of the night to deal with local power outages or network issues.
- Familiar programmability: Applications running in Azure can access data in the share via file system I/O APIs. Developers can therefore use their existing code and skills to migrate existing applications. In addition to System IO APIs, you can use Azure Storage Client Libraries or the Azure Storage REST API.

#### Azure Queues
Azure Queue storage is a service for storing large numbers of messages. Once stored, you can access the messages from anywhere in the world via authenticated calls using HTTP or HTTPS. A queue can contain as many messages as your storage account has room for (potentially millions). Each individual message can be up to 64 KB in size. Queues are commonly used to create a backlog of work to process asynchronously.

Queue storage can be combined with compute functions like Azure Functions to take an action when a message is received. For example, you want to perform an action after a customer uploads a form to your website. You could have the submit button on the website trigger a message to the Queue storage. Then, you could use Azure Functions to trigger an action once the message was received.

#### Azure Disks
Azure Disk storage, or Azure managed disks, are block-level storage volumes managed by Azure for use with Azure VMs. Conceptually, they’re the same as a physical disk, but they’re virtualized – offering greater resiliency and availability than a physical disk. With managed disks, all you have to do is provision the disk, and Azure will take care of the rest.

#### Azure Tables
Azure Table storage stores large amounts of structured data. Azure tables are a NoSQL datastore that accepts authenticated calls from inside and outside the Azure cloud. This enables you to use Azure tables to build your hybrid or multi-cloud solution and have your data always available. Azure tables are ideal for storing structured, non-relational data.


### Azure Migrate

- Azure Migrate is a service that helps you migrate from an on-premises environment to the cloud. Azure Migrate functions as a hub to help you manage the assessment and migration of your on-premises datacenter to Azure. It provides the following:

  - Unified migration platform: A single portal to start, run, and track your migration to Azure.
  - Range of tools: A range of tools for assessment and migration. Azure Migrate tools include Azure Migrate: Discovery and assessment and Azure Migrate: Server Migration. Azure Migrate also integrates with other Azure services and tools, and with independent software vendor (ISV) offerings.
  - Assessment and migration: In the Azure Migrate hub, you can assess and migrate your on-premises infrastructure to Azure.

#### Integrated tools
Azure Migrate hub also includes the following tools to help with migration:

##### Azure Migrate: Discovery and assessment. 
Discover and assess on-premises servers running on VMware, Hyper-V, and physical servers in preparation for migration to Azure.
##### Azure Migrate: Server Migration.
Migrate VMware VMs, Hyper-V VMs, physical servers, other virtualized servers, and public cloud VMs to Azure.
##### Data Migration Assistant. 
Data Migration Assistant is a stand-alone tool to assess SQL Servers. It helps pinpoint potential problems blocking migration. It identifies unsupported features, new features that can benefit you after migration, and the right path for database migration.
##### Azure Database Migration Service. 
Migrate on-premises databases to Azure VMs running SQL Server, Azure SQL Database, or SQL Managed Instances.
##### Web app migration assistant. 
Azure App Service Migration Assistant is a standalone tool to assess on-premises websites for migration to Azure App Service. Use Migration Assistant to migrate .NET and PHP web apps to Azure.
##### Azure Data Box. 
Use Azure Data Box products to move large amounts of offline data to Azure.

#### Azure Data Box
Azure Data Box is a physical migration service that helps transfer large amounts of data in a quick, inexpensive, and reliable way. The secure data transfer is accelerated by shipping you a proprietary Data Box storage device that has a maximum usable storage capacity of 80 terabytes. The Data Box is transported to and from your datacenter via a regional carrier. A rugged case protects and secures the Data Box from damage during transit.

#### Use cases
Data Box is ideally suited to transfer data sizes larger than 40 TBs in scenarios with no to limited network connectivity. The data movement can be one-time, periodic, or an initial bulk data transfer followed by periodic transfers.

Here are the various scenarios where Data Box can be used to import data to Azure.

- Onetime migration - when a large amount of on-premises data is moved to Azure.
- Moving a media library from offline tapes into Azure to create an online media library.
- Migrating your VM farm, SQL server, and applications to Azure.
- Moving historical data to Azure for in-depth analysis and reporting using HDInsight.
- Initial bulk transfer - when an initial bulk transfer is done using Data Box (seed) followed by incremental transfers over the network.
- Periodic uploads - when large amount of data is generated periodically and needs to be moved to Azure.
Here are the various scenarios where Data Box can be used to export data from Azure.

- Disaster recovery - when a copy of the data from Azure is restored to an on-premises network. In a typical disaster recovery scenario, a large amount of Azure data is exported to a Data Box. Microsoft then ships this Data Box, and the data is restored on your premises in a short time.
- Security requirements - when you need to be able to export data out of Azure due to government or security requirements.
- Migrate back to on-premises or to another cloud service provider - when you want to move all the data back to on-premises, or to another cloud service provider, export data via Data Box to migrate the workloads.
Once the data from your import order is uploaded to Azure, the disks on the device are wiped clean in accordance with NIST 800-88r1 standards. For an export order, the disks are erased once the device reaches the Azure datacenter.

#### AzCopy
AzCopy is a command-line utility that you can use to copy blobs or files to or from your storage account. With AzCopy, you can upload files, download files, copy files between storage accounts, and even synchronize files. AzCopy can even be configured to work with other cloud providers to help move files back and forth between clouds.

#### Azure Storage Explorer
Azure Storage Explorer is a standalone app that provides a graphical interface to manage files and blobs in your Azure Storage Account. It works on Windows, macOS, and Linux operating systems and uses AzCopy on the backend to perform all of the file and blob management tasks. With Storage Explorer, you can upload to Azure, download from Azure, or move between storage accounts.

