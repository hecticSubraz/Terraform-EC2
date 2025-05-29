# Terraform EC2 Provisioning

This project provisions an AWS EC2 instance using Terraform.

---

## Files

- `main.tf` — EC2 instance configuration
- `variables.tf` — Input variables
- `outputs.tf` — Public IP and instance ID
- `.gitignore` — Ignores sensitive/state files

---

##  How to Use

1. Set your values in a local `terraform.tfvars` file (this file is not committed):

```hcl
region         = "us-east-1"
ami            = "ami-0c55b159cbfafe1f0"  # Replace with a valid AMI for your region
instance_type  = "t2.micro"
Run the following commands:

terraform init
terraform plan
terraform apply
Type yes when prompted to apply the changes.

 
 🔁 Destroy the Resources
To remove the EC2 instance and all associated resources:

terraform destroy

 Notes
Make sure your AWS credentials are configured using aws configure or environment variables.

Do not commit sensitive files like terraform.tfvars or .terraform/ to version control.

👤 Author
Subraz Thapa
GitHub: hecticSubraz

