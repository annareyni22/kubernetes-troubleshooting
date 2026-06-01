# Useful Kubernetes Commands

## Cluster Information

```bash
kubectl cluster-info
```

## View Nodes

```bash
kubectl get nodes
```

## View Pods

```bash
kubectl get pods
```

## View Pods in All Namespaces

```bash
kubectl get pods -A
```

## Describe Pod

```bash
kubectl describe pod <pod-name>
```

## View Pod Logs

```bash
kubectl logs <pod-name>
```

## Exec Into Pod

```bash
kubectl exec -it <pod-name> -- /bin/bash
```

## View Events

```bash
kubectl get events --sort-by=.metadata.creationTimestamp
```

## View Deployments

```bash
kubectl get deployments
```

## Restart Deployment

```bash
kubectl rollout restart deployment <deployment-name>
```
