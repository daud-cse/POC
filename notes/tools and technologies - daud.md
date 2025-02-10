
### **Technologies and Tools**

Yes, **Docker** and **Kubernetes** are both **technology tools**. Here's a detailed breakdown:

---

### **1. Docker (Dockerize)**  
- **Type**: **Containerization Tool**  
- **Purpose**: Packages applications and their dependencies into lightweight, portable containers.  
- **Key Features**:  
  - Enables consistent environments across development, testing, and production.  
  - Uses Dockerfiles to define container images.  
  - Runs containers on any system with Docker installed.  
- **Example**:  
  - **Local Dockerize**: Running the "Fraud Event API" in a Docker container with Redis for local development.  

---

### **2. Kubernetes**  
- **Type**: **Container Orchestration Tool**  
- **Purpose**: Manages containerized applications at scale, automating deployment, scaling, and operations.  
- **Key Features**:  
  - Manages clusters of containers (e.g., Docker containers).  
  - Provides self-healing, load balancing, and scaling.  
  - Uses manifests (YAML files) to define desired states.  
- **Example**:  
  - **AKS (Azure Kubernetes Service)**: Hosting 88 microservices (e.g., "Tiger Search API") with auto-scaling and high availability.  


### **3. CI/CD & DevOps**
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

### **4. Cloud & Serverless**  
- **Azure Function**:  
  Example: Processing image uploads asynchronously (e.g., resizing images) in a serverless function.  
- **Azure Service Bus**:  
  Example: Asynchronous communication between the "Fraud Event API" and a fraud detection service (using queues/topics).  
- **AKS (Azure Kubernetes Service)**:  
  Example: Hosting 88 containerized microservices (e.g., "Tiger Search API," "Fraud Event API") with auto-scaling.  
- **AKS Configuration**:  
  Example: Configuring ingress controllers, network policies, or pod autoscaling for microservices in AKS.  

---

### **5. Security & Identity**  
- **Azure Key Vault**:  
  Example: Storing secrets (database passwords, API keys) used by the "Authentication and Authorization" service.  
- **Kerberos and LDAP**:  
  Example: Integrating an enterprise Windows Application with on-premises Active Directory for authentication.  
- **Fortify**:  
  Example: Scanning the "Web Application" codebase for security vulnerabilities (e.g., SQL injection).  
- **Authentication and Authorization**:  
  Example: Implementing OAuth2/OIDC for user login in a "Web Application" using Azure AD.  

---

### **6. Monitoring & Testing**  
- **AB Testing**:  
  Example: Testing two UI versions of the "Web Application" to determine which layout increases user engagement.  
- **UnitTest Code (Coverlet)**:  
  Example: Ensuring 80% code coverage for the "Fraud Event API" using xUnit and Coverlet for reports.  
- **SonarCube Analyzer**:  
  Example: Detecting code smells (e.g., duplicated code) in the "Tiger Search API" during PR reviews.  

---

### **7. Event-Driven & Caching**  
- **Redis**:  
  Example: Caching product catalog data in the "Tiger Search API" to reduce database load.  
- **Active Batch**:  
  Example: Scheduling nightly batch jobs (e.g., financial reports) in a legacy Windows Application. 
- **RabbitMQ**:  
  Example: Enabling asynchronous communication between the "Fraud Event API" and a fraud detection service using message queues (e.g., order processing → fraud check).
---

### **8. Applications & Services**  
- **Console Application**:  
  Example: A CLI tool to bulk-import user data into the "Web Service."  
- **Windows Application**:  
  Example: A WPF desktop app for internal employees to manage orders (integrates with "Web Service").  
- **Web Service**:  
  Example: A REST API for managing product inventory (e.g., `GET /api/products`).  
- **Web Application**:  
  Example: A React frontend for an e-commerce platform (calls the "Tiger Search API").  

---

### **9. Project Management**  
- **Maintain Jira Board**:  
  Example: Tracking tasks like "Implement Helm Charts for AKS" in a sprint.  
- **Make Story -> Sprint**:  
  Example: Creating a user story: "As a user, I want to search products by keyword [Tiger Search API]."  

---

### **10. Development Practices**  
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


