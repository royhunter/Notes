## k8s commands

### Cluster
```
$kubectl cluster-info
```

### Node
```bash
$kubectl get nodes
$kubectl describe nodes
```

### Pod
```bash
$kubectl get pods
```

### Deployment
```bash
$kubectl run http --image=katacoda/docker-http-server:latest --replicas=1
$kubectl get deployment
$kubectl describe deployment http

# Create Deployment by using YAML
$kubectl create -f deployment.yaml
# Update YAML
$kubectl apply -f deployment.yaml

```

### Service
```bash
$kubectl get services
$kubectl get svc
$kubectl describe services
$kubectl describe svc svc-name

# Create Service by using YAML
$kubectl create -f service.yaml
```

### Scale
```
$kubectl scale --replicas=3 deployment http
```