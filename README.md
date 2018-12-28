# jaeger-trace-python

Using Jaeger to trace flask & redis based microservices. Below are the steps to run the tracer and services:

1. For a locally set-up cluster, deploy [helm](https://helm.sh/) chart [inside](https://github.com/infracloudio/Jaeger-hackmarathon/tree/master/charts/jaeger-helm) 
```
$ cd charts/jaeger-helm/
$ helm install --name jaeger-trace --debug .
```

2. Check if you are able to access first microservice at `http://localhost:8081/home?item=<any_item_name>`
