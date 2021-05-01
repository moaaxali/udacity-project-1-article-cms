# Overview of Azure compute services
Azure compute is an on-demand computing service for running cloud-based applications.

- Azure Virtual Machines
- Azure App Services

## Azure Virtual Machine
Virtual machines are software emulations of physical computers. They include a virtual processor, memory, storage, and networking resources. VMs host an operating system, and we can install and run software just like a physical computer. When using a remote desktop client, we can use and control the VM as if we were sitting in front of it.

With Azure Virtual Machines, we can create and use VMs in the cloud. VMs provide infrastructure as a service (IaaS) in the form of a virtualized server and can be used in many ways. Just like a physical computer, we can customize all of the software running on the VM. VMs are an ideal choice when we need:

- Total control over the operating system (OS).
- The ability to run custom software.
- To use custom hosting configurations.

Using Virtual Machine reduce costs—up to 72 percent compared to pay-as-you-go prices and give us the power, control, and customization we need at competitive prices. We can minimize cost by following some recommended practices. Before deploying we should know our estimated cost, Azure Calculate our projected costs by using the Pricing calculator and the Total Cost of Ownership (TCO) Calculator. Only add the products, services, and resources that you need for your solution.

Azure VMs can scale from one to thousands of VM instances in minutes with Azure Virtual Machine Scale Sets. We can run single VMs for testing, development, or minor tasks. Or we can group VMs together to provide high availability, scalability, and redundancy. Using Azure virtual machine scale set we can create and manage a group of identical, load-balanced VMs. 

## Azure App Services
With Azure App Service, we can quickly build, deploy, and scale enterprise-grade web, mobile, and API apps running on any platform. We can meet rigorous performance, scalability, security, and compliance requirements while using a fully managed platform to perform infrastructure maintenance. App Service is a platform as a service (PaaS) offering.

App Service enables us to build and host web apps, background jobs, mobile back-ends, and RESTful APIs in the programming language of your choice without managing infrastructure. It offers automatic scaling and high availability. App Service supports Windows and Linux and enables automated deployments from GitHub, Azure DevOps, or any Git repo to support a continuous deployment model.

It allows us to focus on the website and API logic while Azure handles the infrastructure to run and scale our web applications.

With Azure Web App we can save up to 54% vs on-premises and provide flexible pricing option to fit our needs. Using App Service we can meet rigorous, enterprise-grade performance, security and compliance requirements used a trusted, fully managed platform that handles over 40 billion requests per day.

# Azure Compute choice for the *Article CMS project*
After analyzing all the given options for the FlaskWebProject (Articles CMS) and also looking to the nature of the project I finally came to a decision to choose the Azure App Service to deploy it. The are few reasons I choose App Service over VM

- *The first and the important one to choose App service over VM is the ease of management and agility for me*
- *Second, The project is very simple and small that it doesn't require any custom configurations and hence managing and controlling an entire OS for it is somehow a wast of resources.*
- *And Finally, most of the time I use Github for my projects, and this way azure app service will enable me to quickly build and deploy the project using github actions.*


App services are best fit for many scenarios, it enables us to build and host web apps, background jobs, mobile back-ends, and RESTful APIs in the programming language of your choice without managing infrastructure. It provides abstraction from the underlying OS, and Infrastructure which limits us for using extensive set third party softwares and custom configuration. On the other hand VM are best fit when you are about to control the underlying infrastructure for and perform custom configuration for testing and development.