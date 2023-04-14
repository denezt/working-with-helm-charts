# Useful Helm Commands


## Kubernetes Commands
``` sh
# Create a new namespace before beginning
kubectl create ns devops-experiments
```

## Repository
``` sh
# List all available repositories
helm repo list
```

``` sh
# Add a repository
helm add bitnami https://charts.bitnami.com/bitnami
```

``` sh
# Remove a repository
helm repo remove bitnami
```

## Search the Repository
``` sh
# Search a repository
helm search repo mysql
```

``` sh
# Search for databases in all repositories
helm search repo database
```

``` sh
# Search for databases in all repositories
# and display versions
helm search repo database --versions
```

## Install a pod

``` sh
# Initial install of pod
helm install mydb bitnami/mysql
```
``` sh
# Display the status and information from pod
helm status mydb
```

## Advanced Commands
``` sh
# List all available repositories
helm list --namespace NAME_OF_NAMESPACE
```


``` sh

```


``` sh

```


