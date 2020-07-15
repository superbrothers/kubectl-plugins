# kubectl plugins

This repository contains my kubectl plugin scripts.

## How to use them

You can easily get started by following the steps:
```
$ git clone https://github.com/superbrothers/kubectl-plugins.git
$ echo "export PATH=\"${PWD}/kubectl-plugins:\$PATH\"" >> ~/.bashrc
$ source ~/.bashrc
$ kubectl get-all
```

See [Extend kubectl with plugins](https://kubernetes.io/docs/tasks/extend-kubectl/kubectl-plugins/) for more details about kubectl plugin.

## Plugins

| Name                                         | Description                                                                    |
|----------------------------------------------|--------------------------------------------------------------------------------|
| [`kubectl get-all`](./kubectl-get_all)       | List truly all namespaced resources included custom resources (without events) |
| [`kubectl reset-ns`](./kubectl-reset_ns)     | Delete `metadata.namespace` in manifests                                       |
| [`kubectl debug-node`](./kubectl-debug_node) | Create a debugging pod in the node's host namespaces for debugging nodes       |
