
## Changing the role labels on the worker nodes so they come up as workers instead of none when using kubectl get nodes
``` bash
sudo kubectl label node k3s-worker-1 kubernetes.io/role=worker
```
Do the same for k3s-worker-2



