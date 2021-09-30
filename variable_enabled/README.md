# Environment Substitution Manifests

These manifests have environment variables to allow for dynamic deployment.

Example deployment:

```
export TKG_CLUSTER="home-wl1"
envsubst < docker-demo.yml | kubectl apply -f -
envsubst < pacman.yaml | kubectl apply -f -
```
