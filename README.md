run 
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.0/aio/deploy/recommended.yaml

Create a dash-admin-user.yaml file and paste the following:


kubectl apply -f dash-admin-user.yaml

Create dash-clusterrole-yaml file and paste the following:

kubectl apply -f dash-clusterrole.yaml

kubectl proxy

visit http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/


kubectl version

kubectl -n kubernetes-dashboard create token admin-user

if lost reference this link

https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md