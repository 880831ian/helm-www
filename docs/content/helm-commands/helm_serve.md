+++
title = "helm serve"
weight = "38"

tags = ["commands"]
section = "helm-commands"
categories = ["helm-commands"]
type = "page"

slug = "helm-serve"

[menu.main]
  url = "helm-serve"
  parent = "helm-commands"

+++

## helm serve

start a local http web server

### Synopsis



This command starts a local chart repository server that serves charts from a local directory.

The new server will provide HTTP access to a repository. By default, it will
scan all of the charts in '$HELM_HOME/repository/local' and serve those over
the local IPv4 TCP port (default '127.0.0.1:8879').

This command is intended to be used for educational and testing purposes only.
It is best to rely on a dedicated web server or a cloud-hosted solution like
Google Cloud Storage for production use.

See [hosting chart repositories](developing-charts/#chart-repo-guide) for more information on hosting chart repositories in a production setting.


```
helm serve
```

### Options

```
      --address string     address to listen on (default "127.0.0.1:8879")
      --repo-path string   local directory path from which to serve charts
      --url string         external URL of chart repository
```

### Options inherited from parent commands

```
      --debug                     enable verbose output
      --home string               location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string               address of tiller. Overrides $HELM_HOST
      --kube-context string       name of the kubeconfig context to use
      --tiller-namespace string   namespace of tiller (default "kube-system")
```

### SEE ALSO
* [helm](#helm)	 - The Helm package manager for Kubernetes.