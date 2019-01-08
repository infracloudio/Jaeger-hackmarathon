# jaeger-trace-python

Using Jaeger to trace flask & redis based microservices. Below are the steps to run the tracer and services:

1. For a locally set-up cluster, deploy [helm](https://helm.sh/) chart [inside](https://github.com/infracloudio/Jaeger-hackmarathon/tree/master/charts/jaeger-helm) 
```
$ cd charts/jaeger-helm/
$ helm install --name <app-name> --debug .
```

2. Check if you are able to get order_id by passing `http://localhost:<port of main_app.py>/home?item=<any_item_name>`
3. Check if you are able to get order details by passing `http://localhost:<port of main_app.py>/getdetails?order_id=<order_id returned from previous request>`
