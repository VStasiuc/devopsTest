# DevOps Test

## Install NGINX Ingress Controller

Run the following command to install the NGINX Ingress Controller with a `LoadBalancer` service type in the `ingress-nginx` namespace:

```bash
helm install nginx-ingress ingress-nginx/ingress-nginx \
  --set controller.service.type=LoadBalancer \
  -n ingress-nginx --create-namespace
```

## Create a Secret

Run the following command to create the secret:

```bash
kubectl create secret generic veacheslav-secret \
  --from-literal=XMCYBER=IS_THE_BEST \
  -n veacheslav
```
