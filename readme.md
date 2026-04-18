Helm:  Add the aws-ebs-csi-driver Helm repository.
helm repo add aws-ebs-csi-driver https://kubernetes-sigs.github.io/aws-ebs-csi-driver

helm repo update:Install the latest release of the driver.

helm upgrade --install aws-ebs-csi-driver \
    --namespace kube-system \
    aws-ebs-csi-driver/aws-ebs-csi-driver
----------------------------
Grafana:

    helm repo add grafana-community https://grafana-community.github.io/helm-charts

    helm repo list

    helm repo update
    kubectl create namespace monitoring

    helm install roboshop-grafana grafana-community/grafana --namespace monitoring
    
----------------------------------

prometheus:



