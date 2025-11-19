# Deployment and DevOps Essentials — MERN Application

This repository contains my MERN application deployed using cloud hosting and configured with CI/CD, monitoring, and environment management.  
It was completed as part of the **Deployment & DevOps Essentials** assignment.

---

# 🌐 Deployed Application Links

### **Frontend**
🔗 <https://github.com/PLP-MERN-Stack-Development/deployment-and-devops-essentials-lynn004.git>

### **Backend API**
🔗 <https://deployment-and-devops-essentials-lynn004.onrender.com>

---

# 📦 Project Structure

---

# 🚀 CI/CD Pipeline (Render)

This project uses **Render’s auto-deployment pipeline** connected to GitHub.  
Every time I push to the main branch, Render automatically:

1. Pulls the new commit
2. Installs dependencies
3. Builds the backend
4. Deploys the new version
5. Runs health checks

### 📸 CI/CD Screenshots

### **1. Render Build Logs**
Shows installation, build process, and deployment output.  
![Render Build Logs](./screenshots/render-build.png)

### **2. Auto-Deploy Trigger**
Shows Render detecting a new GitHub commit and triggering deployment.  
![Render Auto Deploy](./screenshots/render-deploy.png)

### **3. GitHub → Render Webhook Integration**
Proof of CI/CD connection.  
![GitHub Webhook](./screenshots/webhook.png)

---

# 📊 Monitoring & Logging Setup

Monitoring ensures the application stays healthy and easy to debug.

### **🔧 Monitoring Tools Used**
| Tool | Purpose |
|------|---------|
| **Render Live Logs** | View runtime logs and errors in real time |
| **Render Deploy Logs** | Monitor build and deploy steps |
| **Health Check Endpoint** | Render automatically pings service to verify uptime |
| **Error Logs** | For backend crash and exception tracking |

### 📸 Monitoring Screenshot
![Render Logs](./screenshots/render-logs.png)

---

# 🛠️ Environment Variables

The following environment variables are required:


A `.env.example` file is included in the repo.

---

# ⚙️ Technologies Used

- **MongoDB Atlas**
- **Express.js**
- **React** (if frontend included)
- **Node.js**
- **Render** (Backend Hosting & CI/CD)
- **GitHub** (Source Control)
- **dotenv** (Environment Variables)

---

# 🔄 Deployment Strategy

### **Backend Deployment**
- Hosted on **Render**
- Auto deploys from GitHub main branch
- Connected using GitHub → Render web service

### **Frontend Deployment**
- Hosted on <Vercel / Netlify / Render>  
- Auto deploys on push  
- Uses production environment variables

---

# 📅 Maintenance Plan

- Regular dependency updates  
- Monitor logs weekly  
- Backup MongoDB using Atlas snapshot tools  
- Documented rollback process:  
  - Revert GitHub commit → Render redeploys previous working version

---

# 👤 Author

**Lynn Kurwa**  
Deployment & DevOps Essentials Project

---


