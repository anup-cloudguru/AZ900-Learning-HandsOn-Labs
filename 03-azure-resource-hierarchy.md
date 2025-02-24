## **Chapter 3: Azure Resource Hierarchy**  

Azure organizes resources (e.g., virtual machines, databases) in a **hierarchical structure** to simplify **management, billing, and governance**. This hierarchy ensures **logical grouping and inheritance** of policies, permissions, and configurations.  

---  

### **1. Overview of Azure Resource Hierarchy**  

Azure follows a **top-down approach**, where policies and access control **cascade from higher levels to lower levels**. The hierarchy consists of:  

- **Azure Account** (Root level)  
- **Management Groups** (Optional but useful for organizing multiple subscriptions)  
- **Subscriptions** (Billing and governance boundaries)  
- **Resource Groups** (Logical grouping of related resources)  
- **Resources** (Individual Azure services like VMs, databases, and storage)  

In this chapter, we’ll explore **each component** in detail and **how they interact**.  

---  

### **2. Components of Azure Resource Hierarchy**  

#### **2.1 Azure Account**  
- **Definition**: The **root level** of Azure resources, created upon signing up for Azure.  
- **Key Features**:  
  - Tied to a **Microsoft account** (e.g., Outlook, Hotmail) or an **organizational account**.  
  - **Automatically creates a default subscription** upon signup.  
- **Use Case**: A company’s **Azure account** manages **all cloud resources** for its organization.  

---  

#### **2.2 Management Groups**  
- **Definition**: Containers used to **organize multiple subscriptions** for better governance.  
- **Key Features**:  
  - **Optional** but useful for large organizations.  
  - Supports **nested hierarchy** (e.g., Root → HR → Dev/Prod).  
  - **Policy Inheritance**: Permissions applied at the **root level** cascade down to **child subscriptions**.  
- **Use Case**: Group subscriptions by **department** (e.g., Finance, IT).  

---  

#### **2.3 Subscriptions**  
- **Definition**: Define **billing and governance boundaries** for Azure resources.  
- **Key Features**:  
  - **Mandatory**: At least **one subscription** is required per account.  
  - **Supports multiple subscriptions** for better cost and access control.  
  - Used to separate **environments** (e.g., Dev/Prod) or **departments** (Sales, IT).  
- **Example**: A company may use:  
  - **Subscription 1**: "Sales"  
  - **Subscription 2**: "IT"  

---  

#### **2.4 Resource Groups**  
- **Definition**: **Logical containers** that group related Azure resources.  
- **Key Features**:  
  - A **resource can belong to only one resource group**.  
  - Resource Groups **cannot be nested**.  
  - **Policies and permissions at the resource group level** apply to all resources within it.  
- **Use Cases**:  
  - Separate **environments** (Dev, UAT, Prod).  
  - Group resources by **application** (e.g., Web App + Database).  

---  

#### **2.5 Resources**  
- **Definition**: Individual services deployed in Azure (e.g., **VMs, storage accounts, web apps**).  
- **Key Features**:  
  - The **smallest unit** in the Azure hierarchy.  
  - Each resource must belong to **a single resource group**.  

---  

### **3. Azure Resource Hierarchy Visualization**  

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

### **4. Permissions & Policy Inheritance**  

Azure follows a **top-down approach** for **permissions and policies**:  

| **Hierarchy Level**   | **Policy Example**                   | **Inheritance**                                 |  
|----------------------|------------------------------------|-----------------------------------------------|  
| **Management Group** | Deny public network access        | Applies to all subscriptions under it        |  
| **Subscription**     | Enforce cost limits               | Applies to all resource groups in the subscription |  
| **Resource Group**   | Restrict VM size                  | Applies to all resources in the group        |  

💡 **Example**: A **"deny public IP creation" policy** applied at the **subscription level** prevents **all resource groups under it** from creating public IPs.  

---  

### **5. Key Use Cases**  

✅ **Logical Separation**  
- **Dev vs. Prod**: Use separate **resource groups** for **development** and **production**.  
- **Departmental Isolation**: Assign **subscriptions** to different **departments** (Sales, IT).  

✅ **Cost Management**  
- Track **spending per subscription** or **resource group**.  
- Apply **budget alerts** at the **subscription level**.  

✅ **Security Governance**  
- Assign **permissions** at the **management group level** to streamline access control.  
- Enforce **compliance policies** (e.g., **encryption standards**) across **subscriptions**.  

---  

### **6. Real-World Example: Contoso Corporation**  

Contoso Corporation uses **Azure Resource Hierarchy** as follows:  

📌 **Root Management Group**: "Contoso"  
  - **Child Management Group**: "Finance" (Subscriptions for Payroll & Budgeting).  
  - **Child Management Group**: "IT" (Subscriptions for Dev, UAT, and Prod).  
  - **Resource Groups**:  
    - Under **"IT-Dev" subscription**: "WebApp-Dev," "Database-Dev."  

---  

### **7. Essential Cloud & Azure Terms**  

For a comprehensive list of key cloud and Azure terms, please refer to the [Essential Cloud & Azure Terms](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/blob/main/00-glossary.md).  

---  

### **8. Next Steps**  

In **Chapter 4**, we will explore **Azure Portal Navigation and Free Account Setup**, providing a step-by-step guide on creating a free Azure account and familiarizing yourself with the Azure Portal.
