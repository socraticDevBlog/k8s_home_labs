# istio

istio website: https://istio.io/latest/docs/

### concepts

"Learn about the different parts of the Istio system and the abstractions it uses."

- [traffic managemen](https://istio.io/latest/docs/concepts/traffic-management/)
- security
- observability
- extensability

#### traffic managemenet (networking)

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


