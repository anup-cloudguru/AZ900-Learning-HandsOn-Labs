## **Chapter 1: Introduction to Cloud Computing**  

Welcome to the first chapter of the AZ-900 fundamentals series. This chapter introduces core cloud concepts, laying the groundwork for your journey toward the AZ-900 certification. Whether you're new to Azure or IT in general, this chapter is designed to be beginner-friendly.  

---  

### **1. Overview of AZ-900 Fundamentals**  

The AZ-900 certification covers three main topics:  
- **Cloud Concepts**  
- **Azure Architecture and Services**  
- **Azure Management and Governance**  

In this chapter, our focus is on **Cloud Concepts**. We’ll explain:  
- What cloud computing is  
- The differences between traditional on-premises computing and cloud computing  
- Key service models: IaaS, PaaS, and SaaS  
- The shared responsibility model  
- Basic cost benefits of moving to the cloud  

---  

### **2. What Is Cloud Computing?**  

Cloud computing allows you to use powerful computer resources over the internet without the need for expensive hardware. Instead of purchasing and maintaining physical hardware, you rent what you need from a cloud provider. This approach offers:  

- **Scalability:** Resources can be increased or decreased as needed to meet fluctuating demand, such as handling a sudden surge in website traffic.  
- **Cost Efficiency:** You pay only for what you use, helping businesses avoid high upfront costs.  
- **Flexibility:** Access your services from anywhere with an internet connection, enabling remote work and global collaboration.  

---  

### **3. CAPEX vs. OPEX**  

One of the key benefits of cloud computing is the shift from capital expenditure (CapEx) to operational expenditure (OpEx).  

| **Aspect**        | **On-Premises (CapEx)**                               | **Cloud Computing (OpEx)**                       |  
|-------------------|-------------------------------------------------------|--------------------------------------------------|  
| **Capital Cost**  | High upfront investment (buying hardware, facilities) | Pay-as-you-go pricing; minimal upfront cost       |  
| **Maintenance**   | Customer is responsible for maintenance and upgrades  | Cloud provider handles infrastructure maintenance |  
| **Scalability**   | Limited by physical hardware                           | Elastic and scalable as needed                    |  

This shift reduces the burden of managing physical infrastructure, allowing companies to focus on delivering value through their core business activities.  

---  

### **4. Cloud Service Models**  

Cloud services are generally delivered in one of three models:  

#### **Infrastructure as a Service (IaaS)**  
- **What It Is:** Provides virtualized computing resources over the internet.  
- **Control:** Full control over the operating system, middleware, and applications.  
- **Example:** Azure Virtual Machines, AWS EC2.  
- **Use Case:** An e-commerce company can scale up during peak periods without investing in expensive physical servers.  

#### **Platform as a Service (PaaS)**  
- **What It Is:** Offers a platform and environment for developers to build applications without managing the underlying infrastructure.  
- **Control:** You manage your applications and data, while the provider handles the operating system, runtime, and middleware.  
- **Example:** Azure App Service.  
- **Use Case:** A startup can focus solely on coding while the platform manages servers, storage, and networking.  

#### **Software as a Service (SaaS)**  
- **What It Is:** Delivers software applications over the internet on a subscription basis.  
- **Control:** Minimal control; you simply use the application.  
- **Example:** Office 365, Gmail.  
- **Use Case:** End-users access applications like Google Docs or Microsoft Outlook without worrying about software updates or maintenance.  

| **Service Model** | **You Manage**                | **Provider Manages**                     | **Typical Use Case**                        |  
|-------------------|-------------------------------|------------------------------------------|---------------------------------------------|  
| **IaaS**          | OS, middleware, applications  | Physical infrastructure (servers, storage) | Custom and flexible environments            |  
| **PaaS**          | Applications, data            | OS, runtime, middleware                   | Rapid application development               |  
| **SaaS**          | Limited configuration/data    | Everything else                          | End-user software (e.g., email, CRM)        |  

*IaaS vs. PaaS vs. SaaS Diagram*  
![IaaS vs. PaaS vs. SaaS Diagram](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/blob/main/images/iaas-paas-saas.png)  

---  

### **5. The Shared Responsibility Model**  

Cloud computing operates under a **shared responsibility model** that clearly defines the roles of the cloud provider and the customer.  

- **On-Premises:**  
  *You manage everything—from physical infrastructure to applications.*  

- **Cloud Computing:**  
  - **IaaS:**  
    - **Provider:** Physical hardware, networking, and data center facilities.  
    - **Customer:** Operating system, middleware, applications, and data.  
  - **PaaS:**  
    - **Provider:** Underlying infrastructure, operating system, runtime, and middleware.  
    - **Customer:** Application and data.  
  - **SaaS:**  
    - **Provider:** Almost all aspects of the application, from infrastructure to software updates.  
    - **Customer:** Only data and user-specific configurations.  

#### **Responsibilities Breakdown**  

| Feature                        | On-Premises 🏢 | IaaS 🏗️ | PaaS 🏢 | SaaS 🌐 |  
|--------------------------------|--------------|--------|--------|--------|  
| **Information/Data**           | 🟩 | 🟩 | 🟩 | 🟩 |  
| **Devices (Mobiles/PCs)**      | 🟩 | 🟩 | 🟩 | 🟩 |  
| **Accounts and Identities**    | 🟩 | 🟩 | 🟩 | 🟩 |  
| **Identity & Directory Infrastructure** | 🟩 | 🟩 | 🟨 | 🟨 |  
| **Applications**               | 🟩 | 🟩 | 🟨 | 🟦 |  
| **Network Controls**           | 🟩 | 🟩 | 🟨 | 🟦 |  
| **Operating System**           | 🟩 | 🟩 | 🟦 | 🟦 |  
| **Physical Host**              | 🟩 | 🟦 | 🟦 | 🟦 |  
| **Physical Network**           | 🟩 | 🟦 | 🟦 | 🟦 |  
| **Physical Datacenter**        | 🟩 | 🟦 | 🟦 | 🟦 |  

🟩 = **You Manage**  
🟨 = **Shared Responsibility**  
🟦 = **Cloud Provider Manages**  

💡 **Example:** When migrating an on-premises application to Azure Virtual Machines (IaaS), you retain control over the operating system and the application, while Azure manages the underlying hardware and networking.  

---  

### **6. Lift and Shift Migration**  

**Lift and Shift** refers to moving applications from on-premises environments to the cloud with minimal changes. This approach enables organizations to:  
- Quickly leverage cloud benefits like scalability and cost efficiency.  
- Minimize modifications during migration.  
- Reduce downtime compared to a complete re-architecting of the application.  

💡 **Example:** Migrating a virtual machine running a legacy application from an on-premises data center to Azure Virtual Machines (IaaS) lets you benefit from cloud infrastructure without altering the application. If full cloud optimization is needed—such as auto-scaling or load balancing—a re-architecting approach might be preferable.  

---  

### **7. Essential Cloud & Azure Terms**  

For a comprehensive list of key cloud and Azure terms, please refer to the [Essential Cloud & Azure Terms](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/blob/main/00-glossary.md).  

---  

### **8. Next Steps**  

In **Chapter 2**, we will dive deeper into **Cloud Service Models** and explore the benefits of cloud computing in greater detail, focusing on how these services can be optimized within Azure’s ecosystem.
