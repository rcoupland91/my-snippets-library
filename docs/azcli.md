# AZ CLI Commands

A collection of frequently used Azure CLI commands

!!! info "Prerequisite"
    You must have the Azure CLI installed before running these.

### Authenticate via Device Code
Use this when working on a remote server or a machine without a web browser to log in to your Azure account.
```bash title="Device Login"
az login --use-device-code
```
### Change/Set subscriptions
```bash title="Set Subscription"
az account set --subscription $subscriptionname
```

### Show current context
```bash title="Subscription context"
az account show --output table
```