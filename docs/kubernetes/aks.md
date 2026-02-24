# AKS CLI Commands

```
az login
az account set --subscription <sub>
az aks get-credentials --resource-group <RG> --name <AKS>
```

## Work with network policies
`kubectl get namespace`

`kubectl get netpol -n internal-ingress`

`kubectl get netpol -n internal-ingress internal-ingress -o yaml`

`kubectl get netpol -n <namespace> <pod> -o yaml`

`kubectl get secret`

`kubectl get-pods -n <namespace> `

`kubectl describe pods`

`kubectl logs -n <namespace>`

`kubectl get netpol -n <namespace>  <pod> -o yaml`

`kubectl get namespace`

`kubectl get netpol -n internal-ingress`

`kubectl get secret -n <namespace> `

`kubectl logs -n <namespace>  <pod> `

`kubectl describe pods -n <namespace>  <pod> `

`kubectl get pods -n <namespace> `

## View secret info
`kubectl -n <namespace>  get secret <secret> -o yaml`

## Get cert expiry
`kubectl -n <namespace>  get secret <secret> -o "jsonpath={.data['tls\.crt']}" | base64 -d | openssl x509 -enddate -noout`

## Check full chain in cert
`kubectl get secret db-user-pass -o jsonpath='{.data}'`

The output is similar to using an example random password/username: { "password": "UyFCXCpkJHpEc2I9", "username": "YWRtaW4="}

Decode the password data:

`echo'UyFCXCpkJHpEc2I9'| base64 --decode`