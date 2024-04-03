## DeploymentK8S
### Start pod
kubectl apply -f pod.yml
### See pods
kubectl get pod pod_name
### Delete pods
kubectl delete -f pod.yml
### Start deploy
kuectl apply -f deploy.yml
### See deploy
kubectl get deploy deploy_name
### For more information on replicaset
kubectl get replicaset -o wide

### Create deployment object with cli
kubectl create deployment --image=nginx deployment_object_name
### Scale image
kubectl scale --replicat=2 deployment/deployment_object_name
### Update image
kubectl set image deployment/deployment_object_name container_name=image_name
