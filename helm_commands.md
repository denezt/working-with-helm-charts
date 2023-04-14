# Useful Helm Commands

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

``` sh

```

``` sh

```



