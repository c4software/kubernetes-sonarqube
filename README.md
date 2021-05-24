# kubernetes-sonarqube

Sonarqube in Kubernetes YAML deployment file (tested with K3D)

## Create Kubernetes Cluster

```sh
k3d cluster create --api-port 127.0.0.1:8484 -p "127.0.0.1:42400:80@loadbalancer" --volume $(pwd)/volume/:/mnt/data/ -s 1 -a 2 clusterName
```

## Create Sonarqube pod

```sh
kubectl apply -f deployment-app.yaml
```

Wait the first boot can be long.
