# Deploying to Kubernetes

## Create secrets from .env file

```sh
kubectl create secret generic modmail-env --from-env-file=.env -n apps
```

## Deploy to K8s

```sh
kubectl apply -f ./deploy/k8s/app.yaml 
```