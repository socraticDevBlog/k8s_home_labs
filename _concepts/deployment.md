### Deployment's use cases

- rolling out a ReplicaSet;
- declare a new state of the Pods;
- rollbacking to an earlier Deployment revision;
- scaling up Deployment to facilitate more load;
- pausing the rollout of a Deployment: to apply multiple fixes to its;
  PodTemplateSpec and then resume it to start a new rollout (?)$
- cleaning up old ReplicatSets you don't need animore.

## yml manifest example:

"The following is an example of a Deployment. It creates a ReplicaSet to bring up three nginx Pods"

```yml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        ports:
        - containerPort: 80

```

https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#creating-a-deployment
(2022-12-17)


