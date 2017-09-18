
# Upload kubeconfig

```
export NODE_IP=159.203.167.178
export NODE=kube-01
scp -i ${SSH_KEY} ./gen/${NODE}.kubeconfig ./gen/proxy.kubeconfig root@${NODE_IP}:~/
scp -i ~/development/spc/keys/dev ./gen/${NODE}.kubeconfig ./gen/proxy.kubeconfig root@${NODE_IP}:~/ root@${NODE_IP}:~/
```
