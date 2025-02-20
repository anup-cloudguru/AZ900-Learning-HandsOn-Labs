## **Chapter 6: Azure Virtual Machines**  

### **What is an Azure Virtual Machine (VM)?**  
Azure Virtual Machines (VMs) are **Infrastructure-as-a-Service (IaaS)** offerings that allow users to deploy and manage virtualized servers in the cloud. With full control over the OS and applications, VMs are ideal for custom workloads, development environments, and scalable solutions.  

#### **Key Features**:  
- **Full OS Control**: Install and configure any OS (Windows/Linux) and software.  
- **Scalability**: Scale vertically (upgrade VM size) or horizontally (add more VMs).  
- **Pay-as-You-Go**: Pay only for compute time and storage used.  
- **High Availability**: Integrate with Availability Zones, Availability Sets, or Scale Sets.  

---

### **Creating an Azure Virtual Machine**  

#### **Step-by-Step Guide**:  
1. **Subscription & Resource Group**:  
   - Choose a subscription (e.g., free trial) and create/select a **Resource Group** to organize resources.  
2. **Region & Availability Options**:  
   - Select a **region** (e.g., East US) and configure redundancy using **Availability Zones** or **Availability Sets**.  
3. **VM Configuration**:  
   - **Image**: Choose an OS (e.g., Ubuntu, Windows Server).  
   - **Size**: Select VM specifications (CPU, RAM, disk).  
   - **Authentication**: Use SSH keys (Linux) or passwords (Windows).  
4. **Networking**:  
   - Assign a **public IP** for internet access.  
   - Configure **Network Security Groups (NSGs)** to control inbound/outbound traffic (e.g., open port 22 for SSH).  
5. **Disks**:  
   - **OS Disk**: Choose between HDD, SSD, or premium SSD.  
   - **Data Disks**: Attach additional storage (optional).  
6. **Deployment**:  
   - Review settings, download SSH keys (if applicable), and deploy the VM.  

#### **Example Use Cases**:  
- **Web Hosting**: Deploy a VM to host a website.  
- **Gaming**: Provision high-performance VMs for GPU-intensive games.  

---

### **Benefits of Azure VMs**  
| **Benefit**          | **Description**                                                                 |  
|-----------------------|---------------------------------------------------------------------------------|  
| **Flexibility**       | Customize OS, install software, and configure network settings.                 |  
| **Cost-Effective**    | No upfront hardware costs; pay only for usage.                                  |  
| **Scalability**       | Scale resources up/down based on demand.                                        |  
| **Disaster Recovery** | Replicate VMs across Availability Zones or regions for redundancy.              |  

---

### **Knowledge Check**  
Test your understanding with the following questions:  

1) **You can create a resource group inside another resource group.**  
   ☐ True  
   ☐ False  

2) **A VM can be in multiple resource groups.**  
   ☐ True  
   ☐ False  

3) **A resource group can contain resources from multiple Azure regions.**  
   ☐ True  
   ☐ False  

4) **A resource should be part of one resource group.**  
   ☐ True  
   ☐ False  

5) **You plan to deploy several Azure virtual machines. You need to ensure that the services running on the virtual machines remain available if a single data center fails. What are two possible solutions?**  
   ☐ A. Deploy the virtual machines to two or more availability zones.  
   ☐ B. Deploy the virtual machines to two or more resource groups.  
   ☐ C. Deploy the virtual machines to a scale set.  
   ☐ D. Deploy the virtual machines to two or more regions.  

---

### **Answers & Explanations**  

1) **[✘] False**  
   **Explanation**: Resource groups **cannot be nested**. Each resource group exists independently under a subscription.  

2) **[✘] False**  
   **Explanation**: A VM (or any Azure resource) can belong to **only one resource group**.  

3) **[✔] True**  
   **Explanation**: A resource group can contain resources deployed in **multiple Azure regions**.  

4) **[✔] True**  
   **Explanation**: Every Azure resource must belong to **exactly one resource group**.  

5) **[✔] A. Deploy the virtual machines to two or more availability zones** & **[✔] D. Deploy the virtual machines to two or more regions**  
   **Explanation**:  
   - **A**: Availability Zones protect against **data center failures** within the same region by distributing VMs across physically isolated zones.  
   - **D**: Deploying to multiple regions ensures availability during **region-wide outages**, but this is typically used for broader disaster recovery.  

---

### **Summary**  
- **Resource Groups**: Logical containers for organizing resources (no nesting).  
- **VM Redundancy**: Use Availability Zones for data center failures or multiple regions for regional outages.  
- **Scalability**: Combine VMs with Scale Sets for automatic scaling and load balancing.  

--- 
