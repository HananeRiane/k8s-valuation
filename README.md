# k8s-valuation

#### commands
export KUBECONFIG=../kubeconfig.yml


#### redis deployment
kubectl delete -f redis-deployment.yaml
kubectl apply -f redis-deployment.yaml

#### redis node-deployment
kubectl delete -f redis-node-deployment.yaml
kubectl apply -f redis-node-deployment.yaml


#### service deployment
kubectl delete -f service-redis.yaml
kubectl apply -f service-redis.yaml
kubectl get deployments
kubectl  logs <pod-id>
kubectl get pods


#### multiple deployment
kubectl scale deployment node-redis-hanane --replicas=3
