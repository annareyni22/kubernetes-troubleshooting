# Pending Pods Troubleshooting

## What It Means

The pod has not been scheduled to a node.

## Investigation

### Check Pod Details

```bash
kubectl describe pod <pod-name>
```

### Review Events

Look for messages such as:

* Insufficient CPU
* Insufficient Memory
* Node selector mismatch
* Taints and tolerations issues

### Check Node Resources

```bash
kubectl top nodes
```

### Check Node Status

```bash
kubectl get nodes
```

## Common Causes

* Cluster resource shortage
* Scheduling constraints
* Node not ready
* Storage provisioning issues

## Resolution

* Free resources
* Scale cluster
* Fix node issues
* Review scheduling rules
