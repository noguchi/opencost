# Prometheus for opencost

```
kubectl create ns prometheus
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
helm install my-prometheus prometheus-community/prometheus -n prometheus --create-namespace -f prometheus-custom-values.yaml
```

# opencost

```
kubectl apply -f opencost.yaml
```

# UI

- https://opencost.cluster.noguchi.me/
- https://opencost-prometheus.cluster.noguchi.me/
