## **Chapter 11: Azure App Service**  

### **1. Introduction to Azure App Service**  
Azure App Service is a **Platform-as-a-Service (PaaS)** offering that allows you to host web applications, RESTful APIs, and backend services without managing infrastructure. It supports multiple programming languages and frameworks, providing a **fully managed hosting environment**.  

#### **Key Features:**  
- **Multi-Language Support** → Run apps built with .NET, Java, Python, PHP, Node.js, and more.  
- **Auto-Scaling** → Scale up or out automatically based on demand.  
- **Integrated CI/CD** → Seamless integration with GitHub, Azure DevOps, and Bitbucket.  
- **Built-in Security** → Provides authentication with Azure Active Directory and supports SSL/TLS.  
- **Global Availability** → Deploy applications in multiple Azure regions for redundancy.  

---  

### **2. Types of App Service Plans**  
An **App Service Plan** determines the resources allocated to your web application. Azure provides different tiers based on requirements:

| **Plan Type**   | **Key Features**                                       | **Best For**  |
|---------------|------------------------------------------------|------------|
| **Free (F1)** | Basic hosting, limited resources, no custom domain | Learning, testing |
| **Basic (B1-B3)** | Custom domains, manual scaling, limited features | Small applications |
| **Standard (S1-S3)** | Auto-scaling, staging slots, daily backups | Business applications |
| **Premium (P1-P3)** | High-performance instances, enhanced security | Large-scale apps |
| **Isolated (I1-I3)** | Dedicated environments with enhanced security | Compliance-sensitive apps |

---  

### **3. Deploying an App on Azure App Service**  
Follow these steps to deploy a web application using Azure App Service:

#### **Step 1: Create an App Service**  
1. **Go to Azure Portal** → Search for "App Service" → Click **Create**.
2. **Select Subscription & Resource Group** → Choose an existing one or create a new one.
3. **App Name** → Provide a unique name (e.g., `mywebapp123`).
4. **Runtime Stack** → Choose the preferred framework (e.g., .NET, Python, Java, Node.js).
5. **Region** → Select the nearest Azure region (e.g., East US, West Europe).
6. **App Service Plan** → Choose the appropriate pricing tier.

#### **Step 2: Deploy Code to App Service**  
Azure supports various deployment options:
- **Manual Deployment** → Upload files via the Azure Portal.
- **GitHub Integration** → Enable CI/CD with GitHub Actions.
- **Azure DevOps** → Deploy apps directly from Azure DevOps repositories.
- **ZIP Deploy & FTP** → Upload pre-built applications.

#### **Step 3: Configure Application Settings**  
- Enable **Custom Domains & SSL** for security.
- Configure **Environment Variables**.
- Set up **Scaling Rules** to handle traffic spikes.

#### **Step 4: Test and Monitor the App**  
- **Azure Monitor & Application Insights** provide real-time logs and analytics.
- **Scaling Options** help in handling increased workloads efficiently.

---  

### **4. Azure App Service vs. Virtual Machines (VMs)**  
| Feature | Azure App Service | Virtual Machines (VMs) |
|---------|------------------|------------------|
| **Management** | Fully managed by Azure | Requires manual setup & maintenance |
| **Scaling** | Auto-scaling available | Manual scaling needed |
| **Cost** | Pay for usage; no infrastructure costs | Pay for VM instances, storage, networking |
| **Security** | Built-in security & authentication | Requires manual security configurations |

---  

### **5. Hands-On Project: Deploy a Web App using Azure App Service**  
📌 **Project-5: Deploying a Web App on Azure App Service**  
🔗 *[View Full Project Guide](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/tree/main/Projects_HandsOn/Project-5_Azure-App-Service.md)*  

**Hands-on Activities Covered:**  
✅ **Create an Azure App Service and App Service Plan**  
✅ **Deploy a Web App using GitHub or Azure DevOps**  
✅ **Configure Custom Domains & SSL**  
✅ **Set Up Scaling and Monitoring**  

---  

### **6. Summary**  
✔ **Azure App Service** → A fully managed PaaS for hosting web apps & APIs.  
✔ **App Service Plans** → Defines compute resources allocated to apps.  
✔ **CI/CD Integration** → Supports automated deployments from GitHub & DevOps.  
✔ **Scaling & Security** → Provides auto-scaling, SSL, and authentication.  

---  

### **7. Next Steps**  
💡 *In **Chapter 12: Azure Networking Services (VNET, Subnets, NSG)**, we will explore how Azure networks resources securely and efficiently!* 🚀

