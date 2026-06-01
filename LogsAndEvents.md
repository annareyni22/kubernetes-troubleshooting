# Logs and Events

## View Logs

```bash
kubectl logs <pod-name>
```

## Follow Logs

```bash
kubectl logs -f <pod-name>
```

## Previous Container Logs

```bash
kubectl logs --previous <pod-name>
```

## View Events

```bash
kubectl get events
```

## Sort Events by Time

```bash
kubectl get events --sort-by=.metadata.creationTimestamp
```

## Troubleshooting Approach

1. Check pod status
2. Review events
3. Review logs
4. Check deployment configuration
5. Validate service dependencies
6. Identify root cause
