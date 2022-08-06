# Kubernetes deployment via Helm
Helm chart to deploy a fully functional and secure [`adguard home`](https://github.com/AdguardTeam/AdGuardHome) application in [Kubernetes](https://kubernetes.io/).

## Requirements
Requires a Kubernetes cluster setup, with dns, storage and [Helm and Tiller](https://docs.helm.sh/) configured.

A cluster for testing, can be setup (on Ubuntu) using:
```
snap install microk8s --classic
microk8s.start
microk8s.status --wait-ready
microk8s.enable dns dashboard
microk8s.status --wait-ready
snap install helm --classic
helm init --wait
```

## Updating Values.yaml
If there should be a change to the setup of the config for adguard look at https://github.com/AdguardTeam/AdGuardHome/wiki/Configuration
