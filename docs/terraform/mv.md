How to Import into state with terraform mv (as current resource exists)

```bash
terraform state mv module.testapp_vm module.testapp_vm[0]
```

Or
```bash
terraform state mv module.testapp_vm module.testapp_vm["run"]
``` 
This avoids re-importing and preserves all meta data.