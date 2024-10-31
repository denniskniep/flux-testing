Install current Flux Version
```
curl -s https://fluxcd.io/install.sh | sudo FLUX_VERSION=2.4.0 bash
```

Create Cluster
```
kind create cluster -n linage-test
```

Bootstrap Flux
```
export GITHUB_TOKEN=<my-token>

flux bootstrap github --owner=denniskniep --repository=flux-testing --private=false --personal=true --path=clusters/linage-test/flux
```
