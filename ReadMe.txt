###########################################################################
# We are using "fluentd" namespace in order to deploy fluentd in the cluster
# If it does not exist, prior executing helm, you need to create namespace
###########################################################################
kubectl create namespace fluentd
### fluentd
helm upgrade --install --namespace fluentd clustername-fluentd ./charts/fluentd