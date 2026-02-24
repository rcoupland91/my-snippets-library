# Terraform Init

!!! info "Prerequisite"
    You must have the Terraform installed before running.

```bash
terraform init -backend-config="storage_account_name=example-sa" -backend-config="container_name=example-container" -backend-config="example.tfstate" -backend-config="resource_group_name=example-rg"
```