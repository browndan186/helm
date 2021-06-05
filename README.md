# helm
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
chmod 700 get_helm.sh


./get_helm.sh


helm repo add stable https://charts.helm.sh/stable
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm search repo prometheus-community


Sleep 30

helm install stable prometheus-community/kube-prometheus-stack
