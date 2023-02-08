git add . && git commit -m "initial commit"
git push


## Event straming acroos event hubs



I have SUBSCRIPTION-1 and SUBSCRIPTION-2. I have created an eventhub in SUBSCRIPTION-2. 
I go to SUBSCRIPTION-1 one and create a Resource-Group. 
After creating an Resource-Group, I create a EVENT-GRID. 
Within the eventgrid, I create a EVENT-SUBSCRIPTION that givens an option to point it to an endpoint. 
I chose the endpoint and selected the eventhub that was created in SUBSCRIPTION-1.

##

https://medium.com/kubernetes-tutorials/cluster-level-logging-in-kubernetes-with-fluentd-e59aa2b6093a
https://phoenixnap.com/kb/elasticsearch-kubernetes


Save these manifests in the rbac.yml separating them by the ---delimiter and create all resources in bulk:

kubectl create -f rbac.yml
serviceaccount “fluentd” created
clusterrole.rbac.authorization.k8s.io “fluentd” created
clusterrolebinding.rbac.authorization.k8s.io “fluentd” created


3. Minikube requires a values.yaml file to run Elasticsearch. Download the file with:

curl -O https://raw.githubusercontent.com/elastic/helm-charts/master/elasticsearch/examples/minikube/values.yaml

create