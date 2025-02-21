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
- The difference between traditional on-premises computing and cloud computing
- Key service models: IaaS, PaaS, and SaaS
- The shared responsibility model
- Basic cost benefits of moving to the cloud

---

### **2. What Is Cloud Computing?**

Cloud computing allows businesses and individuals to access computing resources (servers, storage, databases, networking, software) over the internet instead of purchasing and maintaining physical hardware. This approach provides several advantages:

- **Scalability:** Easily increase or decrease resources as needed, such as handling a sudden surge in website traffic during a sale event.
- **Cost Efficiency:** You pay only for what you use, reducing upfront capital costs.
- **Flexibility:** Access your services from anywhere with an internet connection, enabling remote work and global collaboration.

---

### **3. CAPEX vs. OPEX**

One of the key benefits of cloud computing is the shift from capital expenditure (CapEx) to operational expenditure (OpEx).

| **Aspect**          | **On-Premises (CapEx)**                                 | **Cloud Computing (OpEx)**                         |
|---------------------|---------------------------------------------------------|----------------------------------------------------|
| **Capital Cost**    | High upfront investment (buying hardware, facilities)  | Pay-as-you-go pricing; minimal upfront cost        |
| **Maintenance**     | Customer is responsible for maintenance and upgrades    | Cloud provider handles infrastructure maintenance  |
| **Scalability**     | Limited by physical hardware                            | Elastic and scalable as needed                     |

This shift reduces the burden of managing physical infrastructure, allowing companies to focus on their core business activities.

---

### **4. Cloud Service Models**

Cloud services are generally delivered in one of three models:

#### **Infrastructure as a Service (IaaS)**
- **What It Is:** Provides virtualized computing resources over the internet.
- **Control:** Full control over the operating system, middleware, and applications.
- **Example:** Azure Virtual Machines, AWS EC2.
- **Use Case:** An online store can scale up virtual machines during peak shopping seasons without investing in physical servers.

#### **Platform as a Service (PaaS)**
- **What It Is:** Offers a platform for developers to build applications without managing underlying infrastructure.
- **Control:** You manage your applications and data; the provider manages the OS, runtime, and middleware.
- **Example:** Azure App Service.
- **Use Case:** A startup can develop an app using Azure App Service while the platform manages servers and networking.

#### **Software as a Service (SaaS)**
- **What It Is:** Delivers software applications over the internet on a subscription basis.
- **Control:** Minimal control; the provider manages everything.
- **Example:** Office 365, Gmail.
- **Use Case:** Users can access SaaS applications like Google Docs or Dropbox without worrying about installations or updates.

| **Service Model** | **You Manage**                     | **Provider Manages**                             | **Typical Use Case**                       |
|-------------------|------------------------------------|--------------------------------------------------|--------------------------------------------|
| **IaaS**          | OS, middleware, applications       | Physical infrastructure (servers, storage)       | Custom and flexible environments           |
| **PaaS**          | Applications, data                 | OS, runtime, middleware                          | Rapid application development              |
| **SaaS**          | Limited configuration/data         | Everything else                                  | End-user software (e.g., email, CRM)       |

**IaaS vs. PaaS vs. SaaS**  
![IaaS vs. PaaS vs. SaaS Diagram - Placeholder](path/to/image.png "IaaS vs. PaaS vs. SaaS")

---

### **5. The Shared Responsibility Model**

Cloud computing operates under a **shared responsibility model**, defining which components are managed by the provider and which are managed by the customer.

| **Deployment Model** | **You Manage**                           | **Provider Manages**                |
|----------------------|------------------------------------------|-------------------------------------|
| **On-Premises**     | Everything                                | Nothing                            |
| **IaaS**            | OS, middleware, applications, and data   | Hardware, networking, and storage  |
| **PaaS**            | Applications and data                    | OS, runtime, middleware            |
| **SaaS**            | User configurations and data             | Everything else                     |

Example: If you migrate an on-premises app to Azure Virtual Machines (IaaS), you manage the OS and application, while Azure manages hardware and networking.

---

### **6. Lift and Shift Migration**

**Lift and Shift** involves moving applications to the cloud without modifying their architecture. Benefits include:

- Faster migration with minimal changes.
- Immediate access to cloud scalability and cost efficiency.
- Reduced downtime compared to re-architecting.

However, **potential drawbacks** include performance inefficiencies if the app is not optimized for the cloud. In some cases, re-architecting might be required to take full advantage of cloud-native features.

---

### **7. Knowledge Check**

(Quiz questions remain the same)

---

### **8. Essential Cloud & Azure Terms**  
For a comprehensive list of key cloud and Azure terms, check out **[Essential Cloud & Azure Terms](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/blob/main/00-glossary.md)**.

---

### **9. Next Steps**

In **Chapter 2**, we will explore Cloud Service Models in greater detail and discuss how to optimize cloud services within Azure’s ecosystem.
