# Environment Substitution Manifests

These manifests have environment variables to allow for dynamic deployment.

Example deployment:

```
export TKG_CLUSTER="home-wl1"
kubectl create ns docker-demo
envsubst < docker-demo.yml | kubectl -n docker-demo apply -f -

kubectl create ns pacman
envsubst < pacman.yaml | kubectl -n pacman apply -f -
```
