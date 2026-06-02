# ImagePullBackOff Troubleshooting

## What It Means

Kubernetes cannot pull the container image.

## Investigation

### Describe Pod

```bash
kubectl describe pod <pod-name>
```

Look for:

```text
Failed to pull image
ImagePullBackOff
ErrImagePull
```

## Common Causes

### Incorrect Image Name

Verify:

```yaml
image: nginx:latest
```

### Missing Registry Credentials

Check image pull secrets.

### Registry Unavailable

Verify registry connectivity.

### Image Does Not Exist

Confirm image tag exists.

## Resolution

* Correct image name
* Update image tag
* Verify registry credentials
* Verify registry availability
