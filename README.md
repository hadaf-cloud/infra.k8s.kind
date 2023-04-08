# k8s Kind

A Multi Node k8s kind cluster for local development purposes

## Create kind cluster : Run

```sh
kind create cluster --config  cluster-config.yml
```

## Get kubeconfig

```sh
kind get kubeconfig
```

## Untaint control-plane node

untaint control plane node/s to run ingress-nginx example with hostNetwork inyour localhost port 80 in host machine

```sh
kubectl taint nodes --all node-role.kubernetes.io/control-plane-
```

## Delete cluster

```sh
kind delete clusters kind
```

Delet all clusters :

```sh
kind delete clusters --all
```
