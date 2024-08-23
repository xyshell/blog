---
title: CKA Note
date: 2022-01-18 20:16:53
tags: k8s, cka
toc: true
---

# Installation and Configuration

## Intall kubectl

- configuration file location: `$HOME/.kube/config`.

- handy when going from a local environment to a cluster in the cloud, or from one cluster to another, such as from development to production.

```bash
$ kubectl config use-context foobar
```

## GKE Quickstart

1. [GKE Install](https://cloud.google.com/sdk/docs/install#linux)

2. [GKE Quickstart](https://cloud.google.com/kubernetes-engine/docs/quickstart)

3. quick start command

```bash
$ gcloud container clusters create linuxfoundation

$ gcloud container clusters list

$ kubectl get nodes # kubectl comes free from gcloud

$ gcloud container clusters delete linuxfoundation
```

## Minikube

1. [github repo](https://github.com/kubernetes/minikube)

2. install

```bash
$ curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64

$ chmod +x minikube

$ sudo mv minikube /usr/local/bin
```

3. quick start command

```bash
$ minikube start

$ kubectl get nodes
```

## Main Deployment configuration

1. Single-node

With a single-node deployment, all the components run on the same server. This is great for testing, learning, and developing around Kubernetes.

2. Single head node, multiple workers

Adding more workers, a single head node and multiple workers typically will consist of a single node etcd instance running on the head node with the API, the scheduler, and the controller-manager.

3. Multiple head nodes with HA, multiple workers

Multiple head nodes in an HA configuration and multiple workers add more durability to the cluster. The API server will be fronted by a load balancer, the scheduler and the controller-manager will elect a leader (which is configured via flags). The etcd setup can still be single node.

4. HA etcd, HA head nodes, multiple workers

The most advanced and resilient setup would be an HA etcd cluster, with HA head nodes and multiple workers. Also, etcd would run as a true cluster, which would provide HA and would run on nodes separate from the Kubernetes head nodes.
