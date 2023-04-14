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

## Remove a pod
``` sh
# Remove a pod
helm uninstall mydb
```
``` sh
# Remove a pod from a specific namespace
helm uninstall mydb -n NAME_OF_NAMESPACE
```

## Advanced Commands
``` sh
# List all available repositories
helm list --namespace NAME_OF_NAMESPACE
```

``` sh
# How to configure the password to a pod
# using the CLI.
# (NOT FOR PRODUCTION)
helm install mydb bitnami/mysql --set auth.rootPassword="PASSWORD"
```

``` sh
# How to configure the password to a pod
# using the CLI.
# (NOT FOR PRODUCTION)
helm install mydb bitnami/mysql --set auth.rootPassword="PASSWORD"
```


``` sh

```


