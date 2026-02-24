# Terraform Plan/Apply

!!! info "Prerequisite"
    You must have the Terraform installed before running.
    
!!! info "Other articles"
    Please read the other article on tf init [Terraform INIT](init.md)

```bash
terraform plan -var-file="config/global.tfvars" -var-file="config/uks/${environment}/${environment}.tfvars" -lock=false
```