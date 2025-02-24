## **Chapter 12: Azure Networking Services (VNET, Subnets, NSG)**  

### **1. Introduction to Azure Networking**  
Azure Networking Services provide a **secure, scalable, and high-performance** networking infrastructure for Azure workloads. In this chapter, we will cover:  
✅ **Virtual Networks (VNETs)** → Private, isolated networks in Azure.  
✅ **Subnets** → Logical network segments within a VNET.  
✅ **Network Security Groups (NSGs)** → Firewall rules to control inbound/outbound traffic.  

---

### **2. Azure Virtual Network (VNET)**  

#### **What is a VNET?**  
An **Azure Virtual Network (VNET)** is a **private, isolated** network that allows Azure resources to securely communicate with each other and external networks.  

#### **Key Features**  
- **Custom IP Addressing** → Define custom private IP ranges.  
- **Subnets** → Segment networks for better security and performance.  
- **Secure Connectivity** → Use VPNs, ExpressRoute, or Peering.  
- **Traffic Filtering** → NSGs control traffic flow.  

#### **Use Cases**  
- Deploying a **multi-tier application** (Web + App + Database).  
- Connecting on-premises networks to Azure using a **VPN Gateway**.  

---

### **3. Azure Subnets**  

#### **What is a Subnet?**  
A **subnet** is a **smaller network within a VNET** used to organize and control Azure resources.  

#### **Key Features**  
- **Traffic Isolation** → Separate traffic between workloads (e.g., Web, App, DB).  
- **Security** → Apply different NSG rules per subnet.  
- **Scaling** → Optimize performance by segmenting network traffic.  

#### **Example**  
A company deploys:  
- **Subnet-1 (Web Tier)** → Hosts public-facing web servers.  
- **Subnet-2 (App Tier)** → Hosts internal application services.  
- **Subnet-3 (DB Tier)** → Hosts secure databases with restricted access.  

---

### **4. Network Security Groups (NSG)**  

#### **What is an NSG?**  
A **Network Security Group (NSG)** is a **firewall** that controls inbound and outbound traffic to **Azure VMs, Subnets, and Services**.  

#### **How NSGs Work?**  
- **Inbound Rules** → Control incoming traffic (e.g., allow HTTP/HTTPS).  
- **Outbound Rules** → Control outgoing traffic (e.g., restrict internet access).  
- **Priority-Based** → Rules are **evaluated in order (Lowest → Highest)**.  

#### **Example NSG Rules**  
| **Rule**   | **Source**  | **Destination** | **Port**  | **Action** |  
|-----------|------------|---------------|-----------|------------|  
| Allow SSH | Any        | VM1           | TCP 22    | Allow      |  
| Allow HTTP| Any        | Web Server    | TCP 80    | Allow      |  
| Deny All  | Any        | Any           | Any       | Deny       |  

💡 **Best Practice**: Apply **NSGs at the Subnet level** instead of individual VMs for **better management**.  

---

### **5. Hands-On Project: Azure Networking Services**  

📌 **Project-6: Configuring Azure Networking (VNET, Subnets, NSG)**  
🔗 *[View Full Project Guide](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/tree/main/Projects_HandsOn/Project-6_Azure-Networking.md)*  

**Hands-on Activities Covered:**  
✅ **Create a Virtual Network (VNET).**  
✅ **Create Subnets for different workloads.**  
✅ **Configure NSG Rules for security.**  

---

### **6. Summary**  
✔ **Azure VNETs** → Private, isolated cloud networks.  
✔ **Subnets** → Logical divisions within a VNET.  
✔ **NSGs** → Firewall rules for traffic control.  

---

### **7. Next Steps**  
*"In **Chapter 13: Azure Virtual Network Peering & VPN**, we will explore how to securely connect multiple VNETs and extend networks to on-premises data centers."* 🚀
