## **Chapter 6: Azure Virtual Machines**  

### **1. Introduction to Azure Virtual Machines**  
Azure Virtual Machines (VMs) are **Infrastructure-as-a-Service (IaaS)** offerings that allow users to deploy and manage virtualized servers in the cloud. They provide full control over the operating system, software, and networking configurations.  

#### **Key Features:**  
✅ **Full OS Control** → Install and configure any OS (Windows/Linux) and software.  
✅ **Scalability** → Scale vertically (increase VM size) or horizontally (add more VMs).  
✅ **Pay-as-You-Go** → Pay only for compute time and storage used.  
✅ **High Availability** → Ensure reliability with Availability Zones, Availability Sets, or Scale Sets.  

---

### **2. How to Create an Azure Virtual Machine**  

Follow these steps to **provision an Azure VM using the Azure Portal**:  

#### **Step 1: Select Subscription & Resource Group**  
- Choose a **subscription** (e.g., free trial).  
- Create or select a **Resource Group** (e.g., "VM-ResourceGroup").  

#### **Step 2: Configure VM Details**  
- **Region** → Select a region (e.g., **East US**).  
- **Availability Options** → Choose **Availability Zones** for redundancy.  
- **VM Image** → Select an OS (e.g., **Ubuntu, Windows Server**).  
- **VM Size** → Choose specifications (CPU, RAM, Disk).  

#### **Step 3: Set Up Authentication**  
- **Linux** → Use SSH key authentication.  
- **Windows** → Set up a password for RDP access.  

#### **Step 4: Configure Networking**  
- Assign a **public IP** for external access.  
- Set up **Network Security Groups (NSGs)** to allow/deny traffic.  
  - Example: Open **port 22** for SSH (Linux) or **port 3389** for RDP (Windows).  

#### **Step 5: Configure Disks & Storage**  
- Choose between **HDD, SSD, or Premium SSD** for OS Disk.  
- Attach **additional data disks** if needed.  

#### **Step 6: Review & Deploy**  
- Validate settings and **deploy the VM**.  

---

### **3. Key Benefits of Azure Virtual Machines**  

| **Benefit**          | **Description**                                                |  
|----------------------|----------------------------------------------------------------|  
| **Flexibility**      | Customize OS, install software, and configure network settings. |  
| **Cost-Effective**   | No upfront hardware costs; pay only for usage.                 |  
| **Scalability**      | Scale resources up/down based on demand.                       |  
| **Disaster Recovery**| Replicate VMs across **Availability Zones** for redundancy.    |  

---

### **4. Real-World Example**  
💡 **Example**: A **gaming company** provisions **high-performance VMs** for GPU-intensive gaming. After gaming sessions, the company **deallocates the VM**, reducing costs significantly.  

---

### **5. Hands-On Project: Deploy an Azure Virtual Machine**  

📌 **Project-2: Azure Virtual Machine Deployment**  
🔗 [View the Full Project Guide](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/tree/main/Projects_HandsOn/Project-2_Deploying-Azure-VM.md)  

**Hands-on Activities Covered:**  
✅ **Create an Azure Virtual Machine** (Linux & Windows).  
✅ **Access VM via SSH (Linux) or RDP (Windows).**  
✅ **Configure NSG Rules (Allow SSH/RDP).**  

---

### **6. Summary**  
✔ **Azure Virtual Machines** → Provide full OS control in an IaaS environment.  
✔ **Resource Groups** → Logical containers for organizing VMs.  
✔ **Availability Zones** → Protect against data center failures.  

---

### **7. Next Steps**  
*"In **Chapter 7: Azure Virtual Machine Scale Sets & Availability Sets**, we will explore how to scale Azure VMs efficiently and ensure high availability."* 🚀
