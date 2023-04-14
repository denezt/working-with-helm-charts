# Working with MicroK8S

## Kubernetes Commands
``` sh
# Create a new namespace before beginning
microk8s.kubectl create ns devops-experiments
```

``` sh
# Add the Helm3 Addon
microk8s enable helm3
```

## Basic Commands

``` sh
# List all install objects
microk8s helm3 list
```

``` sh
# Install new object
microk8s helm3 install mydb bitnami/mysql
```

``` sh
# Install new object
microk8s helm3 uninstall mydb
```
``` sh
 
```

## Advanced Commands
``` sh
# WARNING: This will remove a persist storage device!!!
# This is required in order to safely remove and reinstall 'mydb' pod
microk8s.kubectl delete pvc data-mydb-mysql-0
```