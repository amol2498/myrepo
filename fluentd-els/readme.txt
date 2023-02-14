
git add . && git commit -m "initial commit"
git push




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
Save these manifests in the rbac.yml separating them by the ---delimiter and create all resources in bulk:

kubectl create -f rbac.yml
serviceaccount “fluentd” created
clusterrole.rbac.authorization.k8s.io “fluentd” created
clusterrolebinding.rbac.authorization.k8s.io “fluentd” created


3. Minikube requires a values.yaml file to run Elasticsearch. Download the file with:

curl -O https://raw.githubusercontent.com/elastic/helm-charts/master/elasticsearch/examples/minikube/values.yaml

#aks-prometheus 
https://techcommunity.microsoft.com/t5/apps-on-azure-blog/using-azure-kubernetes-service-with-grafana-and-prometheus/ba-p/3020459
