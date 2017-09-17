# Control plane

```
export MASTER_IP=159.203.167.178
scp -i ${SSH_KEY} ./gen/ca.pem ./gen/ca-key.pem ./gen/apiserver.pem ./gen/apiserver-key.pem root@${MASTER_IP}:~/
```

# Workers

```
export NODE_IP=159.203.167.178
export NODE=kube-01
scp -i ${SSH_KEY} ./gen/ca.pem ./gen/ca-key.pem ./gen/proxy.pem ./gen/proxy-key.pem ./gen/${NODE}.pem ./gen/${NODE}-key.pem root@${NODE_IP}:~/
scp -i ~/development/spc/keys/dev ./gen/ca.pem ./gen/ca-key.pem ./gen/proxy.pem ./gen/proxy-key.pem ./gen/${NODE}.pem ./gen/${NODE}-key.pem root@${NODE_IP}:~/
```
