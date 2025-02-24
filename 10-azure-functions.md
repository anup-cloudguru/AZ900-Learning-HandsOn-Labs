## **Chapter 10: Azure Functions**  

### **1. Introduction to Azure Functions**  
Azure Functions is a **serverless compute service** that lets you run event-driven code **without managing infrastructure**. It automatically scales based on demand, making it ideal for lightweight, short-lived tasks.  

#### **Key Features:**  
✅ **Serverless Execution** → No need to manage servers or infrastructure.  
✅ **Event-Driven** → Triggered by HTTP requests, timers, queues, or other Azure services.  
✅ **Pay-Per-Use** → Only pay when the function runs (Consumption Plan).  
✅ **Multiple Language Support** → Write in C#, JavaScript, Python, PowerShell, Java, and more.  

---

### **2. How Azure Functions Work**  

Azure Functions execute **in response to triggers**, which are events from **various sources**:  

| **Trigger Type**    | **Description** | **Example Use Case** |  
|--------------------|----------------|----------------------|  
| **HTTP Trigger**   | Runs when an HTTP request is received. | Serverless API, Webhooks |  
| **Timer Trigger**  | Runs at scheduled intervals. | Automated reports, backups |  
| **Queue Trigger**  | Runs when a message is added to an Azure Storage Queue. | Order processing, notifications |  
| **Blob Trigger**   | Runs when a new blob is added to Azure Storage. | Image processing, log analysis |  
| **Event Grid Trigger** | Responds to Azure events (e.g., new VM creation). | Automation workflows |  

💡 **Example:** A **Queue Trigger** function can process new **customer orders** stored in an **Azure Storage Queue**.  

---

### **3. Azure Functions Hosting Plans**  

Azure Functions offers **three pricing/hosting models**:  

| **Plan** | **Scaling** | **Billing** | **Best For** |  
|---------|------------|-------------|-------------|  
| **Consumption Plan** | Automatic | Pay-per-use | Cost-efficient, event-driven workloads |  
| **Premium Plan** | Scales in/out | Per-second billing | High-performance applications |  
| **Dedicated (App Service)** | Manual scaling | Fixed pricing | Long-running workloads |  

💡 **Exam Tip:** If a question asks for **cost-effective scaling**, **Consumption Plan** is the best option!  

---

### **4. Creating an Azure Function**  

#### **Step 1: Navigate to Azure Portal**  
- Go to [Azure Portal](https://portal.azure.com) → Click **Create a Resource** → Search for **Function App**.  

#### **Step 2: Configure Function App**  
- **Subscription & Resource Group** → Choose an existing one or create new.  
- **Function App Name** → Unique name (e.g., `myfunctionapp123`).  
- **Publish Method** → Select **Code** or **Docker Container**.  
- **Runtime Stack** → Choose **.NET, Python, Java, or JavaScript**.  
- **Operating System** → Windows or Linux.  

#### **Step 3: Choose Hosting Plan**  
- Select **Consumption, Premium, or Dedicated Plan**.  
- Click **Review + Create** → Deploy the Function App.  

#### **Step 4: Add a Function**  
- Open **Function App** → Click **+ Create a Function**.  
- Select a **Trigger Type** (e.g., **HTTP Trigger**).  
- Write function code → Save & Test.  

---

### **5. Real-World Example**  
💡 **Example:** A **Timer Trigger** Azure Function automatically **deletes old database records every 24 hours**, reducing storage costs.  

---

### **6. Hands-On Project: Deploying Azure Functions**  

📌 **Project-3: Deploying Azure Functions**  
🔗 *[View Full Project Guide](https://github.com/anup-cloudguru/AZ900-Learning-HandsOn-Labs/tree/main/Projects_HandsOn/Project-4_Azure-Functions.md)*  

💻 **Hands-on Activities Covered:**  
✅ **Create and deploy an Azure Function** using HTTP Trigger.  
✅ **Choose the right hosting plan for your function.**  
✅ **Integrate Azure Functions with Storage and Event Triggers.**  

---

### **7. Summary**  
✔ **Azure Functions** → A serverless compute service for **event-driven automation**.  
✔ **Multiple Triggers** → HTTP, Queue, Timer, Blob, Event Grid, etc.  
✔ **Pay-Per-Use** → **Consumption Plan** is the most cost-effective.  
✔ **Auto-Scaling** → Functions scale dynamically with demand.  

---

### **8. Next Steps**  
*"In **Chapter 11: Azure App Service**, we will explore how to deploy and manage scalable web applications in Azure."* 🚀
