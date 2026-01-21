# Install Minikube

https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fdebian+package

```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb
sudo dpkg -i minikube_latest_amd64.deb
```

# Start Minikube

```
minikube start --addons=ingress
```

# Activate Ingress Addon

```
minikube addons enable ingress
```

# Tunnel Connections

```
minikube tunnel
```

# Install kubectl

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

```
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
```

# Apply namespace

```sh
kubectl apply -f manifests/namespace.yaml
```

# Apply pod

```sh
kubectl apply -f manifests/pod.yaml
```

# Delete pod

```sh
kubectl delete -f manifests/pod.yaml
```

# Apply Deployment

```sh
kubectl apply -f manifests/deployment.yaml
```

# Apply Service

```sh
kubectl apply -f manifests/service.yaml
```

# Apply Ingress

```sh
kubectl apply -f manifests/ingress.yaml
```

# Apply Configmap

```sh
kubectl apply -f manifests/configmap.yaml
```

# Apply Deployment with HTML mounted

```sh
kubectl apply -f manifests/deployment-with-html.yaml
```