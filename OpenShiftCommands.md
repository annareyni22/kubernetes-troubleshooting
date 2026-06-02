# OpenShift Useful Commands

## Login

```bash
oc login
```

## View Projects

```bash
oc projects
```

## Switch Project

```bash
oc project <project-name>
```

## View Pods

```bash
oc get pods
```

## Describe Pod

```bash
oc describe pod <pod-name>
```

## View Logs

```bash
oc logs <pod-name>
```

## View Routes

```bash
oc get routes
```

## View Deployment

```bash
oc get deployment
```

## Execute Inside Pod

```bash
oc rsh <pod-name>
```

## Troubleshooting Checklist

1. Check pod status
2. Review events
3. Review logs
4. Verify route
5. Verify service
6. Validate deployment configuration
