# kubernetes-sonarqube

Sonarqube in Kubernetes YAML deployment file (tested with K3D)

## Volume glitch

To make the stack working you have to manually change the ownership, according the yaml the fsGroup is 999 so :

```sh
sudo chown 999 -R sonarqube-data/
```



