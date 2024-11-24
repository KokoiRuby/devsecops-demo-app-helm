## Overview

The helm chart repo for [devsecops-demo-app](https://github.com/KokoiRuby/devsecops-demo-app).

## Install

An out-of-box Kubernetes cluster environment is required. Try [kind](https://kind.sigs.k8s.io/). 👈 Then set up an [ingress](https://kind.sigs.k8s.io/docs/user/ingress/) controller for it.

```bash
# install
helm install devsecops-demo-app .
```

## Verify

http://localhost/foo

http://localhost/bar

```bash
# or in command line terminal
curl localhost/foo
curl localhost/bar
```

## Uninstall

```bash
helm uninstall devsecops-demo-app
```

