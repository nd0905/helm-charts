# Kubernetes deployment via Helm
Helm chart to deploy a somewhat functional [`twitch-channel-points-miner-v2`](https://github.com/Tkd-Alex/Twitch-Channel-Points-Miner-v2) application in [Kubernetes](https://kubernetes.io/).

Still not fully working because twitch requires addtional input to login.

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

## Value Changes

```
deployment.enviroment.DISCORD_URL
deployment.enviroment.TWITCH_USER
deployment.enviroment.TWITCH_PASS
```
All need to be customized for the chart to deploy.