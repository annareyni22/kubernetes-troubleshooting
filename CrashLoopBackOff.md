# CrashLoopBackOff Troubleshooting

## What It Means

The container starts and repeatedly crashes.

## Investigation Steps

### Check Pod Status

```bash
kubectl get pods
```

### Describe Pod

```bash
kubectl describe pod <pod-name>
```

Review:

* Events
* Container state
* Restart count

### Check Logs

```bash
kubectl logs <pod-name>
```

If multiple containers exist:

```bash
kubectl logs <pod-name> -c <container-name>
```

## Common Causes

* Application startup failure
* Missing environment variables
* Configuration errors
* Database connectivity issues
* Resource constraints

## Resolution

* Review logs
* Verify ConfigMaps and Secrets
* Check image version
* Validate application configuration
* Verify dependent services
