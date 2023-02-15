# README
This repository contains Argo and IaC manifests used for demonstrating the creation and management of
customer networks and deployments.

The repo will have a directory for each tenant. Each tenant directory will follow the same structure.

The following illustration shows the structure for each tenant.

| DIRECTORY | DESCRIPTION | NOTES |
| :--- | :--- | :--- | :--- |
| cloudtacular | Fictional tenant customer *Cloudtacular.io* | |
|   **/argo** | Directory for Argo framework tools | |
|     /cd | ArgoCD working directory | Not currently used; CD data managed in the agent |
|     /events/<app> | Events working directory | Per-app event source manifests |
|     /rollouts | Events working directory | Not currently used |
|     /workflows | Workflow manifests | |
|  **/iac/xplane** | Customer terraform module source | Demo existing TF support |
|    /tf-workspace | Crossplane workspace for its TF provider | Sub-directory per workspace (e.g. dev/prod/qa) |
