# Azure Functions: 
Cloud based compute service that provides event driven and scalable serverless compute for azure. 
Available hosting plans: Consumption, Premium, Dedicated (app service) plan.
You can define triggers that execute your code. Some trigger types are database events, Events, HTTP code, queues.
Bindings are a no code solution for handling input and output data. 
Function App: The context in which your functions run. It’s a unit of deployment, management, and scale for your functions. 
Deployment Slots: Allow your function to run in different instances called slots. Slots let you test a new version of your function in a safe environment then seamlessly swap the new version into production

# Serverless Compute
A Function as a service, or a microservice that is hosted on a cloud platform.
Function timeout is 10 minutes, long functions should be hosted on a VM
If you expect clients to execute your function continuously, a VM might be a cheaper alternative
Only one function app instance can be created every 10 seconds, for up to 200 total instances
# Azure Management Infrastructure
Resource: Basic building block of Azure. VMs, virtual networks, databases.
A single resource can only belong to one resource group
Resource groups provide a convenient way to group resources together.
Azure subscriptions: unit of management, billing, and scale. 
An account can have multiple subscriptions to configure different billing models and apply different access-management policies.
Resources are gathered into resource groups, and resource groups are gathered into subscriptions.
Azure Management Group: Provide a level of scope above subscriptions. You organize subscriptions into containers called management groups and apply governance conditions to the management groups. All subscriptions within a management group automatically inherit the conditions applied to the management group

# Azure Resource Manager (ARM)
Template: The blueprints for your system architecture such as the db and vm
When deploying, the ARM template checks if the resources already exist and are created if not.

# Azure Virtual Machines VM
VMs can be grouped together to provide high availability, scalability, and redundancy. 
The monitoring and management of the vms can be automatic with Scale sets.
Availability sets are designed to ensure that VMs stagger updates and have varied power and network connectivity, preventing you from losing all your VMs with a single network or power failure. VMs can be grouped by the Update domain or Fault domain.
Update Domain groups VMs that can be rebooted at the same time. Only one update domain grouping is offline at a time. 
Fault Domain: groups vms by common power source and network switch. By default, an availability set splits your VMs across up to three fault domains.
There’s no additional cost for configuring an availability set, you only pay for the VMs you create.
There’s no additional cost for configuring an availability set, you only pay for the VMs you create
In the outputs section, you specify value that is returned from deployment. Typically, you return values from resources that were deployed. Limit 64 outputs in a template
VMs can be grouped together to provide


# Azure PowerShell
A command line shell and associated scripting language for most Windows operating systems.
Azure CLI is used to issue a set of commands to add, delete, or modify resources in Azure.
Azure CLI is available in both the Bash and PowerShell sections of Azure Cloud Shell
Azure CLI is used to issue a set of commands to add, delete, or modify resources in Azure. 

# Azure App Services
App Service plans are used to define the resources and capabilities available to the web apps hosted within them. 
A platform-as-a-service that allows developers to build, host, and scale web applications and APIs without managing the underlying infrastructure.

# Azure Git Repo
We can import github repo and transfer all commits and issues
We will have complete history
# Azure Pipelines
Approvals and checks: define a set of validations required before a pipeline or stage runs.
The pipelines library includes secure files and variable groups. Secure files are a way to store files and share them across pipelines

# Azure Repos
Supports various branching models including GitFlow, which is ideal for complex projects with multiple release stages.
Includes branch policies to enforce best practices, such as requiring code reviews or passing builds before merges. 
GitHub
Supports GitHub Flow, a simpler branching strategy ideal for continuous delivery, as well as GitFow for more structured release processes.
Provides branch protection rules that can be configured to engorce status checkes and review processes.
Takeaway: Azure repos offers more structured branching strategies suited for enterprise environments, while GitHub flow is tailored for agile development and continuous integration. 
