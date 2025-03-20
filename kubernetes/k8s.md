# Kubernetes for Beginners

## Introduction to Kubernetes(k8s)

Kubernetes (k8s) is an open-source container orchestration platform that helps in automating the deployments, scaling, and management of containerized applications. The rich feature set of Kubernetes enables it to abstract the underlying infrastructure and manage complex applications at scale. 

K8s is widely used in the industry and it is one of the most famous technologies in the DevOps world. We will cover various topics of k8s in the sections later. You can take reference from the following resources to learn more about Kubernetes -

- [Kubernetes Official Site](https://kubernetes.io/)

- [Kubernetes Blog](https://kubernetes.io/blog/)

- [Kubernetes Fundamentals for Beginners](https://medium.com/the-programmer/kubernetes-fundamentals-for-absolute-beginners-architecture-components-1f7cda8ea536)

## Brief History of Kubernetes

Kubernetes was developed at Google and it was made open-source in 2014. The name Kubernetes comes from the Greek, meaning helmsman or pilot. Kubernetes is the successor to Google's internal container oriented cluster-management system `Borg` - [Read More](https://kubernetes.io/blog/2015/04/borg-predecessor-to-kubernetes/)

Kubernetes fostered from over 15 years of Google's experience of running production workloads at scale.

## Why to use K8s?

Kubernetes helps in orchestration of containerized applications helping in better management, scaling, and automated deployments. K8s is used widely in the industry and has become the de-facto for orchestration of containerized applications. As per the [official documentation](https://kubernetes.io/docs/concepts/overview/#why-you-need-kubernetes-and-what-can-it-do), K8s provides us with the following features -

1. Service Discovery and Load Balancing

2. Storage Orchestration

3. Automated rollouts and rollbacks

4. Automatic bin packing (Fit containers onto the nodes for best utilisation of nodes resources)

5. Self healing in case of contianer failure

6. Secret and configuration management

7. Batch execution

8. Horizontal scaling and IPv4/IPv6 dual stack

9. Designed for extensibility

## Key Concepts & Terminologies of Kubernetes


- **Cluster**: A cluster can be understood as a group on nodes on which the whole kubernetes workload runs.

- **Nodes**: Node is the actual machine on which a Kubernetes workload runs. Node can be a physical or virtual machine which has the underlying hardware resources like memory and cpu to be used for running applications alongside a Kubernetes workload. There are basically two kinds of nodes in K8s cluster - `Master Node` and `Worker Node`.

- **Master Node**: The master node also known as the `primary node` contains the key components that manages the cluster. No appication workloads run on this node. The key components that run on the master node are - API Server (kube-apiserver), Scheduler (kube-scheduler), Controller Manager (kube-controller-manager), Key-Value Store (etcd).

- **Worker Nodes** - The worker nodes also known as `secondary nodes` or simply `nodes` are used to run the actual application workloads in K8s. The worker node resources are managed by the master node.

