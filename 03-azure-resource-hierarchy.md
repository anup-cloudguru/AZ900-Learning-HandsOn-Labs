## **Chapter 3: Azure Resource Hierarchy**  

### **What is Azure Resource Hierarchy?**  
Azure organizes resources (e.g., virtual machines, databases) in a hierarchical structure to simplify management, billing, and governance. This hierarchy ensures logical grouping and inheritance of policies, permissions, and configurations.  

---

### **Components of Azure Resource Hierarchy**  

#### **1. Azure Account**  
- **Definition**: The root level of Azure resources. Created when signing up for Azure.  
- **Key Role**:  
  - Tied to a Microsoft account (e.g., Outlook, Hotmail) or organizational account.  
  - Automatically creates a **default subscription** upon signup.  
- **Example**: A company’s Azure account for managing all cloud resources.  

#### **2. Management Groups**  
- **Definition**: Containers to organize multiple subscriptions.  
- **Key Features**:  
  - **Optional**: Not mandatory but highly recommended for large organizations.  
  - **Hierarchy**: Create nested management groups (e.g., Root → HR → Dev/Prod).  
  - **Policy Inheritance**: Permissions/policies applied at the root level cascade to child subscriptions.  
- **Use Case**: Group subscriptions by department (e.g., Finance, IT).  

#### **3. Subscriptions**  
- **Definition**: Billing and governance boundaries for resources.  
- **Key Features**:  
  - **Mandatory**: At least one subscription is required.  
  - **Multiple Subscriptions**: Organizations often use separate subscriptions for billing, environments (Dev/Prod), or departments.  
  - **Example**: A company uses one subscription for Sales and another for IT.  

#### **4. Resource Groups**  
- **Definition**: Logical containers for grouping related resources.  
- **Key Rules**:  
  - A resource can belong to **only one** resource group.  
  - Resource groups cannot be nested.  
- **Use Cases**:  
  - Separate environments (e.g., Dev, UAT, Prod).  
  - Group resources by application (e.g., Web App + Database).  

#### **5. Resources**  
- **Definition**: Individual services deployed in Azure (e.g., VM, storage account, web app).  
- **Key Role**: The smallest unit in the hierarchy.  

---

### **Hierarchy Visualization**  

```    
Azure Account  
│  
└── Management Groups (Optional)  
    │  
    ├── Subscription 1 (e.g., Dev)  
    │   ├── Resource Group A  
    │   │   ├── Virtual Machine 1  
    │   │   ├── SQL Database 1  
    │   │   └── Storage Account 1  
    │   ├── Resource Group B  
    │       ├── Virtual Machine 2  
    │       ├── Web App 1  
    │       └── Load Balancer 1  
    │  
    └── Subscription 2 (e.g., Prod)  
        ├── Resource Group C  
        └── Resource Group D    
```  

---

### **Permissions and Inheritance**  
Permissions and policies applied at higher levels in the hierarchy **trickle down** to child components.  

| **Level**            | **Policy Example**                | **Inheritance**                                  |  
|-----------------------|------------------------------------|-------------------------------------------------|  
| **Management Group**  | Deny public network access.       | Applies to all subscriptions under it.          |  
| **Subscription**      | Enforce cost limits.              | Applies to all resource groups in the subscription. |  
| **Resource Group**    | Restrict VM size.                 | Applies to all resources in the group.           |  

#### **Example**:  
- A "deny public IP creation" policy at the **subscription level** blocks all resource groups under it from creating public IPs.  

---

### **Key Use Cases**  

#### **1. Logical Separation**  
- **Dev vs. Prod**: Use separate resource groups for development and production environments.  
- **Departmental Isolation**: Assign subscriptions to departments (e.g., Sales, IT).  

#### **2. Cost Management**  
- Track spending per subscription or resource group.  
- Apply budget alerts at the subscription level.  

#### **3. Security Governance**  
- Assign permissions at the management group level to streamline access control.  
- Enforce compliance policies (e.g., encryption standards) across subscriptions.  

---

### **Real-World Example**  
- **Contoso Corporation**:  
  - **Root Management Group**: "Contoso"  
    - **Child Management Group**: "Finance" (with subscriptions for payroll and budgeting).  
    - **Child Management Group**: "IT" (with subscriptions for Dev, UAT, and Prod environments).  
  - **Resource Groups**:  
    - Under "IT-Dev" subscription: "WebApp-Dev," "Database-Dev."  

---

### **Summary**  
- **Azure Account**: Root level with default subscription.  
- **Management Groups**: Organize subscriptions (optional but useful).  
- **Subscriptions**: Billing and governance boundaries.  
- **Resource Groups**: Logical containers for resources.  
- **Resources**: Individual services (e.g., VMs, databases).  

---

### **Knowledge Check**  
Test your understanding with the following questions:  

1) **Management groups provide organizations with the ability to manage the compliance of Azure resources across multiple subscriptions.**  
   ☐ True  
   ☐ False  

2) **Your company plans to migrate to Azure. The company has several departments, and each department's resources will be managed by a department administrator.**  
   **What are two possible techniques to segment Azure for the departments?** *(Each correct answer presents a complete solution.)*  
   ☐ A. Multiple subscriptions  
   ☐ B. Multiple Azure Active Directory (Azure AD) directories  
   ☐ C. Multiple regions  
   ☐ D. Multiple resource groups  

3) **A single Microsoft account can be used to manage multiple Azure subscriptions?**  
   ☐ Yes  
   ☐ No  

4) **Two Azure subscriptions can be merged into a single subscription?**  
   ☐ Yes  
   ☐ No  

5) **You have several virtual machines in an Azure subscription, and you created a new subscription. Which of the following statements are correct?**  
   ☐ VM cannot be moved to a new subscription. **(True/False)**  
   ☐ VM can be moved to a new subscription. **(True/False)**  
   ☐ All VMs can be moved if they are running in the same resource group. **(True/False)**  
   ☐ VM can be moved if they run Windows Server 2016. **(True/False)**  
   ☐ An Azure resource group can contain multiple Azure subscriptions. **(True/False)**  

6) **If you assign permissions for a user to manage the resource group, the user can manage all the Azure resources in that resource group.**  
   ☐ True  
   ☐ False  

7) **If you delete a resource group, all resources inside that resource group will be deleted.**  
   ☐ True  
   ☐ False  

---  

### **Answers & Explanations**  

1) **[✔] True**  
   **Explanation**: **Management Groups** help organizations apply policies and compliance settings across multiple Azure subscriptions. This is useful for enforcing security and governance rules at scale.  

2) **[✔] A. Multiple subscriptions** & **[✔] D. Multiple resource groups**  
   **Explanation**: Using **multiple subscriptions** allows departments to have separate billing and access controls. **Resource Groups** help logically organize and manage related resources, making it easier for department administrators to manage their own resources.  

3) **[✔] Yes**  
   **Explanation**: A single Microsoft account can be used to manage **multiple Azure subscriptions**, which is useful for organizations with different billing needs or environments (e.g., development, testing, production).  

4) **[✘] No**  
   **Explanation**: Two Azure subscriptions **cannot be merged**. However, you can **move some resources** from one subscription to another. Each subscription remains independent.  

5)  
   **[✘] VM cannot be moved to a new subscription. (False)**  
   **[✔] VM can be moved to a new subscription. (True)**  
   **[✘] All VMs can be moved if they are running in the same resource group. (False)**  
   **[✘] VM can be moved if they run Windows Server 2016. (False)**  
   **[✘] An Azure resource group can contain multiple Azure subscriptions. (False)**  

   **Explanation**:  
   - VMs **can be moved** to a new subscription, but **there are restrictions** (e.g., the resource provider must support the move).  
   - All VMs in a resource group **cannot always be moved together**; some resources may have dependencies that prevent them from being moved.  
   - The OS version **does not affect** whether a VM can be moved.  
   - **Resource Groups** belong to a **single subscription**; they **cannot span multiple subscriptions**.  

6) **[✔] True**  
   **Explanation**: If a user has **permissions at the Resource Group level**, they can manage **all resources** inside that group. Azure **Role-Based Access Control (RBAC)** lets you assign permissions at different levels (Subscription, Resource Group, or individual resource).  

7) **[✔] True**  
   **Explanation**: Deleting a **Resource Group** permanently deletes **all the resources inside it**, such as VMs, storage accounts, and databases. **Be cautious** when deleting a Resource Group, as this action **cannot be undone**.  

---
