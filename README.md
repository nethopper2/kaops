# README
This repository contains Argo and IaC manifests used for demonstrating the creation and management of
customer networks and deployments.

The repo will have a directory for each tenant. Each tenant directory will follow the same structure.

The following illustration shows the structure for each tenant.

| DIRECTORY | DESCRIPTION | NOTES |
| :--- | :--- | :--- |
| **cloudtacular** | Fictional tenant customer *Cloudtacular.io* ||
| &emsp;/argo | Directory for Argo framework tools ||
| &emsp;&emsp;&emsp;/cd | ArgoCD working directory | Not currently used; CD data managed in the agent |
| &emsp;&emsp;&emsp;/events/<app> | Events working directory | Per-app event source manifests |
| &emsp;&emsp;&emsp;/rollouts | Events working directory | Not currently used |
| &emsp;&emsp;&emsp;/workflows | Workflow manifests ||
| &emsp;/iac/xplane | Customer terraform module source | Demo existing TF support |
| &emsp;&emsp;&emsp;/tf-workspace | Crossplane workspace for its TF provider | Sub-directory per workspace (e.g. dev/prod/qa)| 
