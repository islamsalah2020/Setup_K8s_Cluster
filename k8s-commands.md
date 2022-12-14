### kubectl apply commands in order

    kubectl apply -f mongo-secret.yml
    kubectl apply -f mongo.yml
    kubectl apply -f mongo-configmap.yml
    kubectl apply -f mongo-express.yml
    kubectl get all

### kubectl get commands

    kubectl get pod
    kubectl get pod --watch
    kubectl get pod -o wide
    kubectl get service
    kubectl get secret
    kubectl get all | grep mongodb

### kubectl debugging commands

    kubectl describe pod mongodb-deployment-xxxxxx
    kubectl describe service mongodb-service
    kubectl logs mongo-express-xxxxxx

### give a URL to external service:
    
    type: LoadBalancer
    externalIPs:
        - 3.88.138.98   (public IP of the node that have the express pod)
