https://phoenixnap.com/kb/elasticsearch-kubernetes


Save these manifests in the rbac.yml separating them by the ---delimiter and create all resources in bulk:

kubectl create -f rbac.yml
serviceaccount “fluentd” created
clusterrole.rbac.authorization.k8s.io “fluentd” created
clusterrolebinding.rbac.authorization.k8s.io “fluentd” created


3. Minikube requires a values.yaml file to run Elasticsearch. Download the file with:

curl -O https://raw.githubusercontent.com/elastic/helm-charts/master/elasticsearch/examples/minikube/values.yaml

create