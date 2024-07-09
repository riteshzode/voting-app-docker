# voting-app-docker-k8s

host docker example-voting-app project by using kubernetes

#### To start the application

Step 1: Apply the deployment

    kubectl apply -f .

Step 2: List deployment and services

    kubectl get all

Step 3: Delete deployment and services

    kubectl delete -f .

Step 4: Port forward service nodeport to localhost or you can try LoadBalancer

    kubectl port-forward svc/vote 8080:80
    kubectl port-forward svc/result 8081:80

