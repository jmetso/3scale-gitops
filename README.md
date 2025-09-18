# 3scale GitOps repository

Multi cluster structure to deploy 3scale

Currently only one cluster configured.

Folder structure:

```
 |____bootstrap
 | |____argocd
 |   |____rhds
 |     |____apps         - argocd apps for rhds cluster overlays
 |     |____app-of-apps  - app-of-apps for rhds cluster argocd apps
 |
 |____clusters
 | |____overlays
 |   |____rhds
 |     |____tst          - rhds cluster overlay for tst env config
 |     |____prd          - rhds cluster overlay for prd env config
 |
 |____components
 | |____apps
 |   |____3scale-apimanager
 |   | |____base         - 3scale base config
 |   |____3scale-operator
 |     |____base         - 3scale  operator base config
 |
 |____environments
   |____overlays
     |____main           - main env overlay for base config

```


Inspired by [https://github.com/gnunn-gitops/standards](https://github.com/gnunn-gitops/standards)
