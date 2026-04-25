# shopnovaorg-helm - main branch (PRODUCTION)

This branch contains Kubernetes manifests for the prod namespace.

## Apply order
```
kubectl apply -f 00-namespaces.yaml
kubectl apply -f 01-gatewayclass.yaml
kubectl apply -f storage/
kubectl apply -f gateway/
kubectl apply -f 01-secrets.yaml
kubectl apply -f 02-configmaps.yaml
kubectl apply -f 03-mongodb.yaml
kubectl apply -f 04-auth-service.yaml
kubectl apply -f 05-product-service.yaml
kubectl apply -f 06-order-service.yaml
kubectl apply -f 07-notification-service.yaml
kubectl apply -f 08-frontend.yaml
kubectl apply -f 09-networkpolicies.yaml
```

The dev branch contains development (dev namespace) manifests.
