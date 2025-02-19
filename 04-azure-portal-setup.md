## **Chapter 4: Azure Portal Navigation and Free Account Setup**  

### **Creating a Free Azure Account**  
To get started with Azure, you can sign up for a **free trial account**, which includes $200 in credits for 30 days and access to popular services for 12 months.  

#### **Steps to Sign Up**:  
1. **Visit the Azure Portal**: Go to [portal.azure.com](https://portal.azure.com) and click **Start Free**.  
2. **Microsoft Account**: Sign in with an existing Microsoft account (e.g., Outlook, Hotmail) or create a new one.  
3. **Verification**:  
   - Enter a phone number for identity verification.  
   - Provide a valid credit/debit card for account validation (*no charges unless you upgrade*).  
4. **Agreements**: Accept Azure’s terms and conditions.  
5. **Activation**: Once verified, your free subscription is activated.  

#### **Key Notes**:  
- The free trial includes **12 months of free services** (e.g., 750 hours of Linux/Windows VMs, 5GB Blob Storage).  
- After 30 days, services continue unless explicitly upgraded to a paid plan.  

---

### **Navigating the Azure Portal**  
The Azure Portal is the web-based interface for managing Azure resources. Below are its key components:  

#### **1. Navigation Menu**  
- Located on the left side.  
- **Key Sections**:  
  - **Home**: Quick access to recent resources.  
  - **All Services**: Browse all Azure services (e.g., Virtual Machines, Storage Accounts).  
  - **Resource Groups**: Logical containers for organizing resources.  
  - **Subscriptions**: View billing and usage details.  

#### **2. Creating Resources**  
You can create resources in three ways:  
| **Method**               | **Description**                                  | **Example**                     |  
|--------------------------|--------------------------------------------------|---------------------------------|  
| **Create a Resource**     | Use the "+ Create a resource" button to deploy services. | Deploying a VM from the marketplace. |  
| **Search Bar**            | Type the resource name (e.g., "Virtual Machine") to start deployment. | Quick access to VM creation. |  
| **Cloud Shell**           | Use command-line tools (Bash/PowerShell) for automation. | Running `az vm create` commands. |  

#### **3. Cloud Shell**  
- **Access**: Click the terminal icon in the top menu bar.  
- **Features**:  
  - **Bash/PowerShell**: Switch between shells as needed.  
  - **Persistent Storage**: Files are saved in a linked Azure Storage Account.  
  - **Built-in Tools**: Pre-installed with Azure CLI, PowerShell modules, and code editors.  

#### **4. Subscriptions and Directories**  
- **Subscriptions**: Billing units tied to your account. Switch between subscriptions (e.g., free trial, paid).  
- **Directories**: Manage Azure Active Directory (AAD) tenants for user access control.  

---

### **Practical Assignment**  
1. **Sign Up**: Create a free Azure account and document the steps.  
2. **Explore the Portal**:  
   - Create a **Resource Group** named "Test-Env".  
   - Deploy a **Linux Virtual Machine** using the portal.  
   - Use **Cloud Shell** to run `az vm list` and verify the VM’s status.  
3. **Share Your Progress**:  
   - Write a blog/LinkedIn post explaining your experience.  
   - Use hashtags: `#AZ900WithPiyush`, `#AzureFundamentals`.  

---

### **Graphics Suggestions**  
1. **Azure Portal Layout**:  
   ```  
   [Dashboard]  
   |  
   ├── Navigation Menu (Left)  
   │   ├── Home  
   │   ├── All Services  
   │   └── Resource Groups  
   |  
   ├── Top Menu Bar  
   │   ├── Cloud Shell  
   │   ├── Notifications  
   │   └── Directory + Subscription  
   |  
   └── Main Workspace (Resource Creation/Management)  
   ```  
2. **Cloud Shell Workflow**:  
   - Diagram showing Cloud Shell → Storage Account → Command Execution.  

---

### **Key Takeaways**  
- **Free Trial**: Leverage 30-day credits and 12-month free services for hands-on practice.  
- **Resource Groups**: Organize resources logically (e.g., by environment or project).  
- **Cloud Shell**: Automate tasks using CLI/PowerShell without local installations.  

---
