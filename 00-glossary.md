# **Essential Cloud & Azure Terms**  

*A collection of essential cloud and Azure computing terms to help understand fundamental concepts.*  

---  

## 📌 **Cloud Concepts**  

- **Cloud Computing**  
  The delivery of computing services (servers, storage, databases, networking, software, etc.) over the internet instead of on-premises infrastructure.  

- **IaaS (Infrastructure as a Service)**  
  A cloud service model providing virtualized computing resources like servers, storage, and networking.  

- **PaaS (Platform as a Service)**  
  A cloud service model offering a platform for developing, running, and managing applications without managing infrastructure.  

- **SaaS (Software as a Service)**  
  A cloud service model where applications are hosted and managed by a provider and accessed via the internet.  

---  

## 💰 **Cost Management**  

- **CapEx (Capital Expenditure)**  
  Upfront investment in physical hardware, software, and infrastructure.  

- **OpEx (Operational Expenditure)**  
  Ongoing costs for cloud services based on a pay-as-you-go model.  

- **Pay-as-You-Go**  
  A pricing model where customers pay only for the resources they use.  

- **Reserved Instances (RI)**  
  A cloud pricing option where customers commit to using a resource for a long-term period (e.g., 1-3 years) for cost savings.  

- **Spot Instances**  
  A discounted pricing model for unused cloud capacity, offering lower prices for non-critical workloads.  

- **Total Cost of Ownership (TCO)**  
  A financial estimate that includes both direct and indirect costs of owning and operating IT infrastructure.  

---  

## 🔐 **Security & Responsibility**  

- **Shared Responsibility Model**  
  A security framework defining responsibilities between the cloud provider and the customer.  

- **Multi-Tenancy**  
  A cloud architecture where multiple customers share the same computing resources securely.  

- **Role-Based Access Control (RBAC)**  
  A system for managing user permissions in Azure at different levels (Subscription, Resource Group, or Resource level).  

- **Azure Policy**  
  A service that enforces security, compliance, and cost control rules (e.g., denying public IP creation).  

- **Least Privilege Principle**  
  A security practice where users are granted the minimum level of access required to perform their tasks.  

- **Azure Lock (Read-Only / Delete Lock)**  
  A feature that prevents accidental deletion or modification of critical resources.  

- **Deny Assignments**  
  A security feature that explicitly blocks actions, even if a user has higher-level permissions.  

---  

## ⚡ **Scalability & Performance**  

- **Scalability**  
  The ability to increase or decrease computing resources as needed.  

- **Vertical Scaling (Scaling Up/Down)**  
  Increasing or decreasing the power of an existing resource (e.g., upgrading a VM's CPU or RAM).  

- **Horizontal Scaling (Scaling Out/In)**  
  Adding or removing instances of a resource (e.g., increasing the number of VMs).  

- **Elasticity**  
  The capability of automatically scaling resources up or down to match demand.  

---  

## 🏗️ **Cloud Migration & Deployment**  

- **Virtual Machine (VM)**  
  A software-based emulation of a physical computer that runs an operating system and applications.  

- **Lift and Shift**  
  A cloud migration strategy where applications are moved to the cloud with minimal changes.  

- **Hybrid Cloud**  
  A computing environment that combines on-premises infrastructure with cloud services.  

- **Public Cloud**  
  Cloud services offered by third-party providers over the internet, available to anyone.  

- **Private Cloud**  
  Cloud computing resources used exclusively by a single organization.  

- **High Availability (HA)**  
  Ensuring that a system remains operational with minimal downtime.  

- **Fault Tolerance**  
  The ability of a system to continue running despite failures (e.g., redundant cloud servers).  

- **Load Balancer**  
  A service that distributes traffic across multiple resources to ensure availability and performance.  

---  

## 🏢 **Azure Resource Hierarchy**  

- **Azure Account**  
  The root-level entity in Azure, linked to a Microsoft or organizational account.  

- **Management Groups**  
  A container used to organize multiple subscriptions and enforce policies at scale.  

- **Subscription**  
  A billing and access boundary for Azure resources. Each Azure Account can have multiple subscriptions.  

- **Resource Group**  
  A logical container for grouping Azure resources. Resources in a group share the same lifecycle.  

- **Resources**  
  Individual Azure services such as Virtual Machines, Storage Accounts, Web Apps, and Databases.  

- **Policy Inheritance**  
  Security settings, access control, and governance rules applied at higher levels (e.g., Management Groups) trickle down to lower levels (e.g., Subscriptions, Resource Groups).  

- **Azure Resource Move**  
  Some Azure resources can be moved between **Resource Groups** or **Subscriptions**, but certain services have restrictions (e.g., Azure SQL Databases cannot be moved).  

- **Billing Scope**  
  Subscriptions define the billing scope—costs are tracked per subscription.  

---  

## 🌐 **Azure Portal & Cloud Shell (NEW from Chapter 4)**  

- **Azure Portal**  
  A **web-based UI** for managing Azure resources, accessible via [portal.azure.com](https://portal.azure.com).  

- **Azure Free Trial**  
  A **$200 credit for 30 days** trial with **12 months of select free services**.  

- **Microsoft Account**  
  An account (e.g., Outlook, Hotmail) required to access Azure services.  

- **Navigation Menu**  
  The **left-side menu** in the Azure Portal that provides access to services like Virtual Machines, Storage, and Subscriptions.  

- **Resource Groups**  
  Logical containers that organize Azure services.  

- **Search Bar**  
  A **quick-access search tool** in the Azure Portal to find resources, services, and settings.  

- **Dashboard**  
  A **customizable** interface in the Azure Portal for monitoring and managing resources.  

- **Azure Cloud Shell**  
  A **browser-based command-line interface** for managing Azure resources using Bash or PowerShell.  

- **Azure CLI**  
  A command-line tool that allows users to manage Azure resources programmatically.  

- **Subscriptions**  
  Azure **billing and access control units** that define pricing and resource limits.  

- **Azure Active Directory (AAD)**  
  Microsoft's cloud-based **identity and access management service** used for authentication and authorization.  

---

## ☁️ **Azure & Cloud Services**  

- **Azure**  
  Microsoft’s cloud computing platform offering various services, including IaaS, PaaS, and SaaS.  

- **Azure VPN Gateway**  
  A cloud service that connects on-premises networks to Azure securely.  

- **Azure Arc**  
  A hybrid cloud management tool that allows managing on-premises, multi-cloud, and edge environments from Azure.  
