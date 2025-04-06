# secure-k8s-deployment-with-ghcr-and-rbac
“This project demonstrates a secure Kubernetes application deployment using a private container image hosted on GitHub Container Registry (GHCR). It uses a ServiceAccount with imagePullSecrets and fine-grained RBAC permissions to control pod access and adhere to best practices in Kubernetes security.”

📁 Updated Folder Structure:
├── Dockerfile
├── README.md
├── k8s/
│   ├── namespace.yaml
│   ├── secret-create.sh
│   ├── serviceaccount.yaml      
│   ├── role-rbac.yaml           
│   └── deployment.yaml     

🔐 k8s/serviceaccount.yaml

📜 k8s/role-rbac.yaml

🚀 k8s/deployment.yaml

✅ Deployment Steps
1. Create Namespace & Secret
kubectl apply -f k8s/namespace.yaml
bash k8s/secret-create.sh

2. Apply ServiceAccount + RBAC
kubectl apply -f k8s/serviceaccount.yaml
kubectl apply -f k8s/role-rbac.yaml

3. Deploy Application
kubectl apply -f k8s/deployment.yaml

###
🏆 Now Your Project Is Legit
You can now confidently list this in your CV as:
Secure Kubernetes Deployment using GHCR, ServiceAccounts, and RBAC

📌 Highlights:
Pulled private container image from GHCR using imagePullSecrets
Created a custom ServiceAccount with minimal RBAC permissions
Secured workload identity and automated access to private registries
Debugged and resolved ImagePullBackOff issue using kubectl describe, token scopes, and namespace scoping
###

### 
💼 On Your CV or GitHub
Project: k8s-ghcr-private-deployment
Summary:
Implemented secure Kubernetes deployment using private container images from GitHub Container Registry (GHCR). Configured namespace-scoped ServiceAccount with imagePullSecrets and Role-Based Access Control (RBAC) to follow best practices for workload identity, access, and image authentication 
###
