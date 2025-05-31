# medusa-terraform-deploy
# Medusa


# 🚀 Medusa Terraform Deployment on AWS ECS Fargate

This project automates the deployment of the [Medusa](https://medusajs.com/) open-source headless commerce backend on AWS ECS using Terraform. It includes complete infrastructure-as-code setup with scalable container deployment and CI/CD.

---

## 🛠️ Tech Stack

- **Infrastructure as Code:** Terraform
- **Cloud Provider:** AWS (ECS Fargate, ALB, IAM, RDS)
- **Containerization:** Docker
- **CD Pipeline:** GitHub Actions (optional)
- **Backend:** Medusa.js (Node.js)

---

## 📁 Project Structure

```bash
.
├── my-medusa-store/             # Medusa backend code
├── terraform/                   # Terraform files for AWS infrastructure
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   ├── backend.tf
│   └── provider.tf
└── README.md


#######
** Set up AWS Credentials**

export AWS_ACCESS_KEY_ID="your-access-key"
export AWS_SECRET_ACCESS_KEY="your-secret-key"

########
########

** Initialize and Apply Terraform **
bash
Copy code
cd terraform
terraform init
terraform plan
terraform apply

#########
#########

**Build and Push Docker Image**

docker build -t medusa-backend .
docker tag medusa-backend:latest <your-ECR-repo-url>:latest
docker push <your-ECR-repo-url>:latest

#########
```
--------------------------- * HAppY CoDiNg * ------------------------------ 

````

