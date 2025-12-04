# CloudOps Dashboard - DevOps + AIOps + GreenOps

A unified dashboard demonstrating modern DevOps practices with AIOps, GreenOps, and Multi-Cloud integration, designed for OpenShift deployment.

## 🚀 Features

### **DevOps**
- CI/CD pipeline simulation
- Real-time deployment metrics
- Automated testing visualization
- Incident tracking and management

### **AIOps**
- Intelligent anomaly detection
- Predictive analytics and forecasting
- Automated remediation workflows
- Machine learning pattern recognition

### **GreenOps**
- Energy-efficient dark mode
- Carbon footprint tracking
- Resource optimization
- Eco-friendly design patterns

### **Multi-Cloud**
- AWS, Azure, GCP, OpenShift integration
- Unified cloud management
- Cross-cloud optimization
- Health monitoring dashboard

## 📋 Prerequisites

- OpenShift Cluster (4.10+)
- GitHub Account
- Git CLI (optional)

## 🛠️ Deployment to OpenShift

### Method 1: From Developer Console
1. Login to OpenShift Console
2. Click "+Add" → "Import from Git"
3. Paste your GitHub URL: `https://github.com/YOUR-USERNAME/cloudops-dashboard`
4. Select "Node.js" builder
5. Click "Create"

### Method 2: Using CLI
```bash
# Create new app
oc new-app nodejs:18-ubi8~https://github.com/YOUR-USERNAME/cloudops-dashboard

# Expose the service
oc expose svc/cloudops-dashboard

# Get route URL
oc get route cloudops-dashboard
