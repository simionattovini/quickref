# Kubernetes

## Useful commands

### See Available Contexts

```bash
kubectl config get-contexts
```

### Use a context

```bash
kubectl config use-context <context_id>
```

### List pods and their statuses

```bash
watch kubectl get pods -n <context_id>
```
> `watch` is a linux command that will run the command ahead every 2 seconds and refresh the screen.

### Set namespace into session

```bash
kubectl config set-context --current --namespace=<namespace_id>
```
> This is so that you don't have to use `-n <context_id>` everytime.

### List logs from a pod

```bash
kubectl logs -f <pod_id>
```

### List jobs from a context

```bash
watch kubectl get jobs -n <context_id>
```

### Describe a pod

```bash
kubectl describe pod <pod_id>
```

### Join kube config files into one

```bash
kubectl config view --flatten > ~/.kube/<filename>
```
