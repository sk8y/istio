# istio
istio installation

#  steps

- download istioctl
```
$ curl -L https://istio.io/downloadIstio | sh -

$ <path>/istioctl install --set profile=default -y 

$ istioctl ps

$ k get ns

$ k get po -n istio-system
```

- add label to namespace, to allow sidecar injection
```
$ kubectl label namespace test-app istio-injection=enabled 
```
