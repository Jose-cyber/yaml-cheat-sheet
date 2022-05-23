# Multiples yaml's files using YAML.

This is an exemple of multiples yamls files, you have to use this "---" to separate files, for exemple:

<pre>

apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx
spec:
  replicas: 10
  selector:
    matchLabels:
      app: server
  template:
    metadata:
      labels:
        app: server 
    spec:
      containers:
      - name: nginx-container
        image: nginx:latest
        ports:
        - containerPort: 80
---
apiVersion: v1
kind: Service 
metadata:
  name: nginx-service
spec:
  type: ClusterIP
  ports:
  - protocol: TCP
    name: http-svc 
    port: 80
  selector:
    app: server
</pre>

# [<< home](../README.md)