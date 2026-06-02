# OOMKilled Troubleshooting

## What It Means

The container exceeded its memory limit and was terminated by Kubernetes.

## Investigation

### Check Pod Status

```bash
kubectl describe pod <pod-name>
```

Look for:

```text
Reason: OOMKilled
```

### Check Resource Limits

```bash
kubectl describe deployment <deployment-name>
```

### Check Current Usage

```bash
kubectl top pod
```

## Common Causes

* Memory leak
* Insufficient memory limits
* Large workload
* Unexpected traffic spike

## Resolution

* Increase memory limits
* Optimize application
* Investigate memory leaks
* Scale application if needed
