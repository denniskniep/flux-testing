```
kind create cluster -n linage-test
```

```
export GITHUB_TOKEN=<my-token>

flux bootstrap github --owner=denniskniep --repository=flux-testing --private=false --personal=true --path=clusters/linage-test/flux
```
