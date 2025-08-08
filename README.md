# TASK 3: Infrastructure as Code (IaC) with Terraform

## 🎯 Objective:
Provision a **local Docker container** using **Terraform** to understand the Infrastructure as Code (IaC) workflow.

---

## 🛠️ Tools Used:
- **Terraform** v1.12.2
- **Docker** v28.3.2
- OS: Windows 10 (using Git Bash)

## ⚙️ Steps Performed:

1. ✅ Created `main.tf`
Used `kreuzwerker/docker` provider to:
- Pull the `nginx:latest` Docker image
- Provision a container named `terraform-nginx`
- Map container port `80` to host port `8080`

2. ✅ Initialized Terraform
terraform init

3. ✅ Planned Infrastructure
terraform plan

4. ✅ Applied Configuration
terraform apply
Confirmed nginx was running at: http://localhost:8080

5. ✅ Verified Terraform State
terraform state list
Output:
docker_container.nginx
docker_image.nginx

6. ✅ Destroyed Infrastructure
terraform destroy


✅ Outcome:
Successfully:

Provisioned and deployed a Docker container using Terraform

Verified container from browser (localhost:8080)

Destroyed resources using terraform destroy