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

Cloud computing lets you use powerful computer resources over the internet without buying and maintaining expensive hardware. Instead of purchasing and maintaining expensive hardware, you rent what you need from a cloud provider. This approach enables:

- **Scalability:** Resources can be increased or decreased as needed to meet fluctuating demand, such as handling a sudden surge in website traffic during a sale event.
- **Cost Efficiency:** You pay only for what you use, helping businesses avoid the high upfront costs of on-premises infrastructure and offering flexibility for startups or small businesses.
- **Flexibility:** Access your services from anywhere with an internet connection, enabling remote work or global collaboration without worrying about location-specific limitations.

---

### **3. CAPEX vs. OPEX**

One of the key benefits of cloud computing is the shift from capital expenditure (CapEx) to operational expenditure (OpEx).

| **Aspect**          | **On-Premises (CapEx)**                                 | **Cloud Computing (OpEx)**                         |
|---------------------|---------------------------------------------------------|----------------------------------------------------|
| **Capital Cost**    | High upfront investment (buying hardware, facilities)  | Pay-as-you-go pricing; minimal upfront cost        |
| **Maintenance**     | Customer is responsible for maintenance and upgrades    | Cloud provider handles infrastructure maintenance  |
| **Scalability**     | Limited by physical hardware                            | Elastic and scalable as needed                     |

This shift helps companies reduce the burden of managing physical infrastructure and focus more on delivering value through their core business activities.

---

### **4. Cloud Service Models**

Cloud services are generally delivered in one of three models:

#### **Infrastructure as a Service (IaaS)**
- **What It Is:** Provides virtualized computing resources over the internet.
- **Control:** Full control over the operating system, middleware, and applications.
- **Example:** Azure Virtual Machines, AWS EC2.
- **Use Case:** An e-commerce company running an online store on Amazon EC2 or Microsoft Azure Virtual Machines can scale up during holiday sales and scale down when traffic is low. They don’t have to invest in expensive physical servers.

#### **Platform as a Service (PaaS)**
- **What It Is:** Offers a platform and environment for developers to build applications without managing the underlying infrastructure.
- **Control:** You manage your applications and data, while the provider manages the OS, runtime, and middleware.
- **Example:** Azure App Service.
- **Use Case:** A startup developing a mobile app can use Azure App Service or Google App Engine to build and deploy their app. The developers focus only on coding while the platform handles the servers, storage, and networking.

#### **Software as a Service (SaaS)**
- **What It Is:** Delivers software applications over the internet on a subscription basis.
- **Control:** Minimal control; you simply use the application.
- **Example:** Office 365, Gmail.
- **Use Case:** Google Docs, Dropbox, or Microsoft Outlook are great examples of SaaS. Users can access them from any device without installing software or managing updates—the provider takes care of everything..

| **Service Model** | **You Manage**                     | **Provider Manages**                             | **Typical Use Case**                       |
|-------------------|------------------------------------|--------------------------------------------------|--------------------------------------------|
| **IaaS**          | OS, middleware, applications       | Physical infrastructure (servers, storage)       | Custom and flexible environments           |
| **PaaS**          | Applications, data                 | OS, runtime, middleware                           | Rapid application development              |
| **SaaS**          | Limited configuration/data         | Everything else                                  | End-user software (e.g., email, CRM)         |

---

### **5. The Shared Responsibility Model**

Cloud computing operates under a **shared responsibility model**. This model clearly defines which parts of the system are managed by the cloud provider and which parts are the customer’s responsibility.

- **On-Premises:**  
  *You manage everything—from physical infrastructure to applications.*

- **Cloud Computing:**
  - **IaaS:**  
    - **Provider:** Physical hardware, networking, and data center facilities.  
    - **Customer:** Operating system, middleware, applications, and data.
  - **PaaS:**  
    - **Provider:** Underlying infrastructure, OS, runtime, and middleware.  
    - **Customer:** Application and data.
  - **SaaS:**  
    - **Provider:** Almost all aspects of the application, from infrastructure to software updates.  
    - **Customer:** Only data and user-specific configurations.

*Example:* When migrating an on-premises application to Azure Virtual Machines (IaaS), you retain control over the operating system and the application, while Azure manages the underlying hardware and networking.

---

### **6. Lift and Shift Migration**

**Lift and Shift** refers to moving applications from on-premises environments to the cloud without redesigning them. This approach allows organizations to:

- Leverage cloud benefits (scalability, cost-efficiency) quickly.
- Minimize changes to the application during migration.
- Reduce downtime compared to full re-architecting.

💡 **Example:** Migrating a virtual machine running a legacy application from an on-premises data center to Azure Virtual Machines (IaaS). The application remains unchanged but benefits from cloud infrastructure.

However, **Lift and Shift** may not always be the best option if you need to fully optimize an application for the cloud. In such cases, a **re-architecting** approach may be necessary to take full advantage of cloud-native features like auto-scaling, load balancing, and managed services.

---

### **7. Knowledge Check**

Test your understanding with the following questions:

1) **When you are implementing a Software as a Service (SaaS) solution, you are responsible for configuring the SaaS solution. Everything else is managed by the cloud provider.**  
   ☐ True  
   ☐ False  

2) **You plan to migrate a web application to Azure that is accessed by external users. You need to recommend a cloud deployment solution to minimize the amount of administrative effort used to manage the web application. What should you choose?**  
   ☐ A. IaaS  
   ☐ B. PaaS  
   ☐ C. SaaS  
   ☐ D. DaaS  

3) **PaaS provides full control over the operating system.**  
   ☐ True  
   ☐ False  

4) **Your company plans to deploy a custom application to Azure that will have several prerequisite applications and services installed. Which cloud service should you recommend?**  
   ☐ A. IaaS  
   ☐ B. PaaS  
   ☐ C. SaaS  

5) **In SaaS, the customer is responsible for software updates.**  
   ☐ True  
   ☐ False  

6) **You must have physical servers to use in Cloud Computing.**  
   ☐ True  
   ☐ False  

7) **SQL Server hosted on the cloud and updates managed by Azure is provided as which service?**  
   ☐ A. IaaS  
   ☐ B. PaaS  
   ☐ C. SaaS  

8) **MSSQL Server 2019 installed on a VM is considered PaaS.**  
   ☐ True  
   ☐ False  

9) **You plan to use Azure to host two apps named App1 and App2. The apps must meet the following requirements:**  
   - You must be able to modify the code of App1.  
   - Administrative effort to manage the operating system for App1 must be minimized.  
   - App2 must run interactively with the operating system of the server.  
   **Which type of cloud service should you use for each app?**  
   ☐ A. IaaS  
   ☐ B. PaaS  
   ☐ C. SaaS  
   *(Answer format: e.g., App1: [Service], App2: [Service])*  

10) **You have an application that uses a legacy database, and you plan to move the app to the cloud. Which cloud service would you use?**  
    ☐ A. IaaS  
    ☐ B. PaaS  
    ☐ C. SaaS  

---

### **Answers & Explanations**

1) **[✔] True**  
   **Explanation:** In SaaS, customers configure the solution (e.g., users, settings) while the provider manages the infrastructure, operating system, and updates.

2) **[✔] B. PaaS**  
   **Explanation:** PaaS abstracts the infrastructure and OS management, allowing developers to focus on the application code, thus minimizing administrative effort for external-facing web applications.

3) **[✔] False**  
   **Explanation:** In PaaS, the cloud provider manages the operating system, runtime, and environment. Customers focus on applications and data.

4) **[✔] A. IaaS**  
   **Explanation:** IaaS provides full control over the operating system and allows you to install prerequisite applications and services, making it ideal for custom applications requiring specific configurations.

5) **[✔] False**  
   **Explanation:** In SaaS, software updates and maintenance are managed by the cloud provider, not the customer.

6) **[✔] False**  
   **Explanation:** Cloud computing uses virtualized resources, so you do not need to own or manage physical servers.

7) **[✔] B. PaaS**  
   **Explanation:** Managed SQL Server offerings (e.g., Azure SQL Database) are provided as PaaS, where Azure handles updates and maintenance.

8) **[✔] False**  
   **Explanation:** Installing MSSQL Server 2019 on a VM requires you to manage the operating system and updates, classifying it as an IaaS solution rather than PaaS.

9) **Answer:**  
   - **App1:** PaaS  
   - **App2:** IaaS  
   **Explanation:** App1 benefits from minimized OS management (PaaS) while still allowing code modifications, whereas App2 requires full control of the operating system, making IaaS the appropriate choice.

10) **[✔] A. IaaS**  
    **Explanation:** Legacy applications often require specific configurations and full control over the environment, which is best provided by IaaS.

---

### **8. Essential Cloud & Azure Terms**  
For a comprehensive list of key cloud and Azure terms, check out **[Essential Cloud & Azure Terms](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/blob/main/00-glossary.md)**.

---

### **9. Next Steps**

In **Chapter 2**, we will dive deeper into Cloud Service Models and explore the benefits of cloud computing in greater detail, focusing on how these services can be optimized within Azure’s ecosystem.
