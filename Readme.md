# Changedetection.io Kubernetes Deployment

- Deployed in its own namespace
- Persistent storage using NFS PVC
- Exposed via Service + Ingress
- Readiness and Liveness checks
- Resource limits

## To deploy:
- Edit the ip address and paths of the NFS directory in pvc-data.yaml
- Customize the ingress hostname
- Apply the namespace first with `kubectl apply -f ns/namespace.yaml`
- Deploy the project with `kubectl apply -f .`

---
This deployment demonstrates concepts such as namespaces, persistent storage, services, ingress, and pod health checks.