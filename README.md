# jaeger-trace-python
Using Jaeger to trace flask & redis based microservices. The project is deployed with the help of helm package installer. Below are the steps to run the tracer and services:

1. For a locally set-up cluster, using helm inside Jaeger-hackmarathon/jaeger-trace/:
helm install --name jaeger-trace --debug .

2. Check if you are able to access first microservice at http://localhost:8081/home
