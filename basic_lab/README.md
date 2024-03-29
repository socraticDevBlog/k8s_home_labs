# basic k8s lab with Minikube and Istio

## requirements

- Docker engine is installed and running
- Install Minikube to your local machine: [follow instructions on Minikube's website](https://minikube.sigs.k8s.io/docs/start/)

## lab process

0. Start a Minikube instance and set required resources values
   ```bash
    minikube start --cpus 4 --memory 16384
   ```
1. [install istio](https://istio.io/latest/docs/setup/getting-started/#download) using istioctl
2. stay on the same page and deploy the sample application (bookstore)

## istio

istio website: https://istio.io/latest/docs/

### concepts

"Learn about the different parts of the Istio system and the abstractions it uses."

- [traffic management](https://istio.io/latest/docs/concepts/traffic-management/)
- security
- observability
- extensability

### traffic managemenet (networking)

[Envoy is an open source edge and service proxy, designed for cloud-native
applications](https://www.envoyproxy.io/)

[architecture
overview](https://istio.io/latest/docs/ops/deployment/architecture/)

i.e. flow of traffic and API calls between services

istio makes kubernetes internal networking more reliable against failures

circuit breakers; timeouts and retries; A/B testing; canary rollouts and staged roll-outs; 

Envoy proxies: all traffic within the service mesh (data plane traffic) gets
proxied through Envoy. Relying on Envoy permits you to control traffic around
the mesh without changing your services.



