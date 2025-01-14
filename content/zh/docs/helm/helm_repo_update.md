---
title: "Helm 仓库更新"
---

## helm repo update

从chart仓库中更新本地可用chart的信息

### 简介

更新从各自chart仓库中获取的有关chart的最新信息。信息会缓存在本地，被诸如'helm search'等命令使用。

你可以指定需要更新的仓库列表。
    $ helm repo update <repo_name> ...
使用 'helm repo update' 更新所有仓库。

```shell
helm repo update [REPO1 [REPO2 ...]] [flags]
```

### 可选项

```shell
      --fail-on-repo-update-fail   update fails if any of the repository updates fail
  -h, --help   help for update
```

### 从父命令继承的命令

```shell
      --debug                       enable verbose output
      --kube-apiserver string       the address and the port for the Kubernetes API server
      --kube-as-group stringArray   group to impersonate for the operation, this flag can be repeated to specify multiple groups.
      --kube-as-user string         username to impersonate for the operation
      --kube-ca-file string         the certificate authority file for the Kubernetes API server connection
      --kube-context string         name of the kubeconfig context to use
      --kube-token string           bearer token used for authentication
      --kubeconfig string           path to the kubeconfig file
  -n, --namespace string            namespace scope for this request
      --registry-config string      path to the registry config file (default "~/.config/helm/registry/config.json")
      --repository-cache string     path to the file containing cached repository indexes (default "~/.cache/helm/repository")
      --repository-config string    path to the file containing repository names and URLs (default "~/.config/helm/repositories.yaml")
```

### 请参阅

* [helm repo](helm_repo.md) - 添加、列出、删除、更新和索引chart仓库
