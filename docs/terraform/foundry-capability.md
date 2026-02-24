# Delete Capability Host
When creating a capability host with foundry.  A default host tends to deploy itself without any settings defined.

To deploy this in code, we need to remove the capability host auto-created.

```bash
az rest --method get --url "https://management.azure.com/subscriptions/<SUB_ID>/resourceGroups/<RG_NAME>/providers/Microsoft.CognitiveServices/accounts/<ACCOUNT_NAME>/capabilityHosts?api-version=2025-06-01"
az rest --method delete --url "https://management.azure.com/subscriptions/<SUB_ID>/resourceGroups/<RG_NAME>/providers/Microsoft.CognitiveServices/accounts/<ACCOUNT_NAME>/capabilityHosts/<capability_host_name>?api-version=2025-06-01"
```