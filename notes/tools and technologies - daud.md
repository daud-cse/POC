
### **Technologies and Tools**


### **1. CI/CD & DevOps**
- **ADO Pipeline (Azure DevOps Pipeline)**:  
  Example: Automatically build and deploy microservices to AKS when code is pushed to the `main` branch.  
- **Argo CD**:  
  Example: GitOps-driven deployment to AKS, syncing Kubernetes manifests from a Git repository.  
- **HELM Chart**:  
  Example: Packaging a microservice (e.g., "Fraud Event API") with its dependencies (Redis, configs) for deployment to AKS.  
- **Canary Deployment**:  
  Example: Rolling out a new version of the "Tiger Search API" to 5% of users first to monitor performance.  
- **Blue-Green Deployment**:  
  Example: Switching traffic from the old "Web Service" (blue) to the new version (green) with zero downtime.  

---

### **2. Cloud & Serverless**  
- **Azure Function**:  
  Example: Processing image uploads asynchronously (e.g., resizing images) in a serverless function.  
- **Azure Service Bus**:  
  Example: Asynchronous communication between the "Fraud Event API" and a fraud detection service (using queues/topics).  
- **AKS (Azure Kubernetes Service)**:  
  Example: Hosting 88 containerized microservices (e.g., "Tiger Search API," "Fraud Event API") with auto-scaling.  
- **AKS Configuration**:  
  Example: Configuring ingress controllers, network policies, or pod autoscaling for microservices in AKS.  

---

### **3. Security & Identity**  
- **Azure Key Vault**:  
  Example: Storing secrets (database passwords, API keys) used by the "Authentication and Authorization" service.  
- **Kerberos and LDAP**:  
  Example: Integrating an enterprise Windows Application with on-premises Active Directory for authentication.  
- **Fortify**:  
  Example: Scanning the "Web Application" codebase for security vulnerabilities (e.g., SQL injection).  
- **Authentication and Authorization**:  
  Example: Implementing OAuth2/OIDC for user login in a "Web Application" using Azure AD.  

---

### **4. Monitoring & Testing**  
- **AB Testing**:  
  Example: Testing two UI versions of the "Web Application" to determine which layout increases user engagement.  
- **UnitTest Code (Coverlet)**:  
  Example: Ensuring 80% code coverage for the "Fraud Event API" using xUnit and Coverlet for reports.  
- **SonarCube Analyzer**:  
  Example: Detecting code smells (e.g., duplicated code) in the "Tiger Search API" during PR reviews.  

---

### **5. Event-Driven & Caching**  
- **Redis**:  
  Example: Caching product catalog data in the "Tiger Search API" to reduce database load.  
- **Active Batch**:  
  Example: Scheduling nightly batch jobs (e.g., financial reports) in a legacy Windows Application. 
- **RabbitMQ**:  
  Example: Enabling asynchronous communication between the "Fraud Event API" and a fraud detection service using message queues (e.g., order processing → fraud check).
---

### **6. Applications & Services**  
- **Console Application**:  
  Example: A CLI tool to bulk-import user data into the "Web Service."  
- **Windows Application**:  
  Example: A WPF desktop app for internal employees to manage orders (integrates with "Web Service").  
- **Web Service**:  
  Example: A REST API for managing product inventory (e.g., `GET /api/products`).  
- **Web Application**:  
  Example: A React frontend for an e-commerce platform (calls the "Tiger Search API").  

---

### **7. Project Management**  
- **Maintain Jira Board**:  
  Example: Tracking tasks like "Implement Helm Charts for AKS" in a sprint.  
- **Make Story -> Sprint**:  
  Example: Creating a user story: "As a user, I want to search products by keyword [Tiger Search API]."  

---

### **8. Development Practices**  
- **Local Dockerize**:  
  Example: Running the "Fraud Event API" in Docker Compose with Redis for local development.  
- **GitSquash -> Git Desktop**:  
  Example: Squashing 10 messy commits into one before merging a feature into `main` via Git Desktop.  

---

### **Example Workflow**  
1. **Development**: Build a "Fraud Event API" (ASP.NET Core) and test locally using **Local Dockerize** (with Redis).  
2. **CI/CD**: Use **ADO Pipeline** to build, run **UnitTest Code**, scan with **SonarCube**, and deploy to **AKS** via **HELM Chart**.  
3. **Deployment**: Roll out the API using **Canary Deployment** on AKS, monitored via Argo CD.  
4. **Security**: Store API keys in **Azure Key Vault** and enforce **Authentication** with OAuth2.  
5. **Monitoring**: Use AB Testing to validate the API’s impact on fraud detection rates.  



### **Technology--Azure Kubernetes Service (AKS)** 

**Tools**:

  1. **Azure CLI (Command-Line Interface)**: A tool to manage AKS clusters and other Azure resources through command-line commands. You can use it to create, configure, and scale AKS clusters.
  
  2. **kubectl**: A Kubernetes command-line tool used to interact with and manage Kubernetes clusters. It’s commonly used to deploy applications, inspect cluster resources, and troubleshoot issues in AKS.
  
  3. **Azure Portal**: The web-based interface that provides a visual way to manage AKS clusters and resources in Azure, including scaling clusters, configuring networking, and monitoring.
  
  4. **Azure Monitor**: A service that provides monitoring capabilities for AKS, including logs, metrics, and alerts to track the health and performance of your Kubernetes clusters and workloads.
  
  5. **Helm**: A package manager for Kubernetes that simplifies the deployment and management of applications on AKS using pre-configured charts (packages).
  
  6. **Azure DevOps**: A suite of tools that can be integrated with AKS to automate the build, deployment, and management of Kubernetes applications using CI/CD pipelines.
  
  7. **Kubernetes Dashboard**: A web-based UI that allows you to manage and troubleshoot applications running in AKS clusters.
  
  8. **Azure Security Center**: Provides security management and threat protection for AKS clusters, helping to monitor and protect the workloads running within them.
  
  8. **K9s**: Provides security management and threat protection for AKS clusters, helping to monitor and protect the workloads running within them.

These are some of the tools that integrate with and enhance the usage of AKS as part of the overall cloud-native architecture and container management.

In .NET development, **technology** and **tools** serve different purposes but are closely related:  

### **Technology**  
- Refers to the **frameworks, platforms, and programming languages** used to build applications.  
- Defines the **architecture, design patterns, and methodologies** for software development.  
- Examples in .NET:  
  - **ASP.NET Core** (for web applications)  
  - **Entity Framework Core** (for ORM and database access)  
  - **Razor** (for building interactive web UIs)  
  - **Microservices Architecture**
  - **GIT OPS**  

### **Tools**  
- Refers to **software applications and utilities** that assist in the development, debugging, deployment, and maintenance of .NET applications.  
- Helps developers **write, test, and manage** code efficiently.  
- Examples in .NET:  
  - **Visual Studio / Visual Studio Code** (IDE for development)  
  - **NuGet** (package manager for .NET libraries)  
  - **Azure DevOps / GitHub Actions** (for CI/CD and version control)  
  - **Postman** (for testing APIs)  
  - **SonarQube** (for static code analysis)  
  - **Docker & Kubernetes** (for containerization and orchestration)  

### **Key Difference**  
- **Technology** is what you use to **develop** applications (e.g., ASP.NET Core).  
- **Tools** are what you use to **support** development, debugging, and deployment (e.g., Visual Studio, NuGet).  

Let me know if you need more details! 🚀
