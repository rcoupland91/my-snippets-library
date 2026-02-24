# Use kubectl exec to login to pod

```
kubectl -n <namespace> get pods -o wide | grep <pod>
```
```
kubectl -n <namespace> exec -it <pod> -- /bin/bash
```