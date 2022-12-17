# kubernetes (k8s) concepts

## Deployment

"A Deployment provides declarative updates for Pods and ReplicaSets."

* we don't manage ReplicaSets owned by Deployments

> You describe a desired state in a Deployment, and the Deployment Controller
> changes the actual state to the desired state at a controlled rate. You can
> define Deployments to create new ReplicaSets, or to remove existing
> Deployments and adopt all their resources with new Deployments.

[more...](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#creating-a-deployment)

## ReplicaSets

"A ReplicaSet's purpose is to maintain a stable set of replica Pods running at
any given time. As such, it is often used to guarantee the availability of a
specified number of identical Pods."

> A ReplicaSet ensures that a specified number of pod replicas are running at any given time. However, a Deployment is a higher-level concept that manages ReplicaSets and provides declarative updates to Pods along with a lot of other useful features. Therefore, we recommend using Deployments instead of directly using ReplicaSets, unless you require custom update orchestration or don't require updates at all.

[more...](https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/#example)
