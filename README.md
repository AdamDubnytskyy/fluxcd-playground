# GitOps with FluxCD

## FluxCD bootstrap for GItHub
1. generate [GitHub PAT](https://fluxcd.io/flux/installation/bootstrap/github/#github-pat)
2. Run the [bootstrap for a repository](https://fluxcd.io/flux/installation/bootstrap/github/#github-personal-account) on your personal GitHub account:
```sh
flux bootstrap github \
  --token-auth \
  --owner=my-github-username \
  --repository=my-repository-name \
  --branch=main \
  --path=clusters/my-cluster \
  --personal
```
