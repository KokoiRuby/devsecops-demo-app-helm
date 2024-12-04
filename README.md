## Overview

The helm chart repo for [devsecops-demo-app](https://github.com/KokoiRuby/devsecops-demo-app). There is also a [twin](https://github.com/KokoiRuby/devsecops-demo-app-helm-argocd-pr) repo that you will meet later as you are going through the tutorial

## Install

An out-of-box Kubernetes cluster environment is required. Try [kind](https://kind.sigs.k8s.io/). 👈 Then set up an [ingress](https://kind.sigs.k8s.io/docs/user/ingress/) controller for it.

```bash
# install
helm install devsecops-demo-app .
```

Add local DNS resolution.

```bash
# Windows: C:\Windows\System32\drivers\etc
# WSL: sudo vim /etc/hosts
127.0.0.1 demo-app.default.devsecops.yukanyan.us.kg
```

## Verify

http://demo-app-dev.devsecops.yukanyan.us.kg/foo

http://demo-app-dev.devsecops.yukanyan.us.kg/bar

```bash
# or in command line terminal
curl demo-app-dev.devsecops.yukanyan.us.kg/foo
curl demo-app-dev.devsecops.yukanyan.us.kg/bar
```

## Uninstall

```bash
helm uninstall devsecops-demo-app
```

