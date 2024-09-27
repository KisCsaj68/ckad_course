## Lecture:
- Service for internal and external communications
- external communication -> NodePortService
- virtual server inside the node 
- Service type : Nodeport, ClusterIP, LoadBalancer

  - NoderPort: targetPort on the pod -> the service distribute the requests to this port, NodePort (30000 - 32767) access the webserver externally
   - with the selector property we are able to attach pods to services. you have to use the same labelas as selectors as in the pod definition file

 - CLusterIP : with this easy to communicate between microservices pods by the names