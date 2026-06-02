# Services and Networking Troubleshooting

## Check Services

```bash
kubectl get svc
```

## Describe Service

```bash
kubectl describe svc <service-name>
```

## Verify Endpoints

```bash
kubectl get endpoints
```

A service without endpoints usually means:

* Pods are not running
* Label selectors do not match

## Verify Pod Labels

```bash
kubectl get pods --show-labels
```

## Test Connectivity from a Pod

```bash
kubectl exec -it <pod-name> -- /bin/bash
```

Inside the pod:

```bash
curl http://service-name
```

## DNS Resolution

```bash
nslookup service-name
```

## Common Issues

* Service selector mismatch
* Application not listening on expected port
* DNS resolution failure
* Network policy restrictions
* Pod not ready

## Troubleshooting Flow

1. Check pod status
2. Check service
3. Check endpoints
4. Verify labels
5. Test connectivity
6. Review logs
