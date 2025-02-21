## **Chapter 1: Introduction to Cloud Computing**

Welcome to the first chapter of the AZ-900 fundamentals series. This chapter introduces core cloud concepts, laying the groundwork for your journey toward the AZ-900 certification. Whether you're new to Azure or IT in general, this chapter is designed to be beginner-friendly.

---

## **1. Overview of AZ-900 Fundamentals**

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

## **2. What Is Cloud Computing?**

Cloud computing is a model for accessing computing resources (servers, storage, databases, networking, software, etc.) over the Internet on an on-demand basis. Instead of purchasing and maintaining expensive hardware, you rent what you need from a cloud provider. This approach enables:

- **Scalability:** Resources can be increased or decreased as needed to meet fluctuating demand, such as handling a sudden surge in website traffic during a sale event.
- **Cost Efficiency:** You pay only for what you use, helping businesses avoid the high upfront costs of on-premises infrastructure and offering flexibility for startups or small businesses.
- **Flexibility:** Access your services from anywhere with an internet connection, enabling remote work or global collaboration without worrying about location-specific limitations.

---

## **3. CAPEX vs. OPEX**

One of the key benefits of cloud computing is the shift from capital expenditure (CapEx) to operational expenditure (OpEx).

| **Aspect**          | **On-Premises (CapEx)**                                 | **Cloud Computing (OpEx)**                         |
|---------------------|---------------------------------------------------------|----------------------------------------------------|
| **Capital Cost**    | High upfront investment (buying hardware, facilities)  | Pay-as-you-go pricing; minimal upfront cost        |
| **Maintenance**     | Customer is responsible for maintenance and upgrades    | Cloud provider handles infrastructure maintenance  |
| **Scalability**     | Limited by physical hardware                            | Elastic and scalable as needed                     |

This shift helps companies reduce the burden of managing physical infrastructure and focus more on delivering value through their core business activities.

---

## **4. Cloud Service Models**

Cloud services are generally delivered in one of three models:

### **Infrastructure as a Service (IaaS)**
- **What It Is:** Provides virtualized computing resources over the internet.
- **Control:** Full control over the operating system, middleware, and applications.
- **Example:** Azure Virtual Machines, AWS EC2.
- **Use Case:** Ideal when you need customizable computing environments or want to migrate legacy systems to the cloud without re-architecting them.

### **Platform as a Service (PaaS)**
- **What It Is:** Offers a platform and environment for developers to build applications without managing the underlying infrastructure.
- **Control:** You manage your applications and data, while the provider manages the OS, runtime, and middleware.
- **Example:** Azure App Service.
- **Use Case:** Ideal for application development when you want to focus on writing code rather than managing infrastructure, and need rapid application development and deployment.

### **Software as a Service (SaaS)**
- **What It Is:** Delivers software applications over the internet on a subscription basis.
- **Control:** Minimal control; you simply use the application.
- **Example:** Office 365, Gmail.
- **Use Case:** Perfect for end-users who need ready-to-use software without worrying about maintenance or updates, such as email services, CRMs, and productivity tools.

| **Service Model** | **You Manage**                  | **Provider Manages**                     | **Typical Use Case**                    |
|-------------------|---------------------------------|------------------------------------------|-----------------------------------------|
| **IaaS**         | OS, middleware, applications    | Physical infrastructure (servers, storage) | Custom and flexible environments        |
| **PaaS**         | Applications, data              | OS, runtime, middleware                  | Rapid application development           |
| **SaaS**         | Limited configuration/data      | Everything else                          | End-user software (e.g., email, CRM)    |

---

## **5. The Shared Responsibility Model**

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

To illustrate: If you're migrating an on-premises application to Azure Virtual Machines (IaaS), you retain control over the operating system and the application, while Azure is responsible for the underlying hardware and networking.

---

## **6. Lift and Shift Migration**

**Lift and Shift** refers to moving applications from on-premises environments to the cloud without redesigning them. This approach allows organizations to:

- Leverage cloud benefits (scalability, cost-efficiency) quickly.
- Minimize changes to the application during migration.
- Reduce downtime compared to full re-architecting.

💡 **Example:** Migrating a virtual machine running a legacy application from an on-premises data center to Azure Virtual Machines (IaaS). The application remains unchanged but benefits from cloud infrastructure.

However, **Lift and Shift** may not always be the best option if you need to fully optimize an application for the cloud. In such cases, a **re-architecting** approach may be necessary to take full advantage of cloud-native features like auto-scaling, load balancing, and managed services.

---

### **7. Knowledge Check**

Test your understanding with the following questions:

1) **When implementing a Software as a Service (SaaS) solution, you are responsible for configuring the SaaS solution while everything else is managed by the cloud provider.**  
   ☐ True  
   ☐ False  

2) **You plan to migrate a web application to Azure that is accessed by external users. To minimize administrative effort, which cloud deployment solution should you choose?**  
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

---

### **Answers & Explanations**

1) **[✔] True**  
   **Explanation:** In SaaS, customers configure the solution (e.g., users, settings) but do not manage infrastructure, OS, or updates, which are handled by the provider.

2) **[✔] B. PaaS**  
   **Explanation:** PaaS abstracts the infrastructure and OS management, allowing developers to focus on the application code and user interface, minimizing administrative effort for external-facing applications.

3) **[✔] False**  
   **Explanation:** In PaaS, the cloud provider manages the OS, runtime, and environment. Customers control applications and data, but do not manage the underlying OS.

4) **[✔] A. IaaS**  
   **Explanation:** IaaS provides full control over the OS and allows the installation of prerequisite applications and services, making it suitable for custom applications requiring specific configurations.

---

## **8. Next Steps**

In **Chapter 2**, we will dive deeper into Cloud Service Models and explore the benefits of cloud computing in greater detail, focusing on how these services can be optimized within Azure’s ecosystem.
