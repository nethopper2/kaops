# README
This repository contains Argo and IaC manifests used for demonstrating the creation and management of
customer networks and deployments.

The repo will have a directory for each tenant. Each tenant directory will follow the same structure.

The following illustration shows the structure for each tenant.

| DIRECTORY | DESCRIPTION | NOTES |
| :--- | :--- | :--- |
| **cloudflow** | Fictional tenant customer *Cloudflow* ||
| &emsp;/argo | Directory for Argo framework tools ||
| &emsp;&emsp;&emsp;/cd | ArgoCD working directory | Not currently used; CD data managed in the agent |
| &emsp;&emsp;&emsp;/events/<app> | Events working directory | Per-app event source manifests |
| &emsp;&emsp;&emsp;/rollouts | Events working directory | Not currently used |
| &emsp;&emsp;&emsp;/workflows | Workflow manifests ||
| &emsp;/iac/crossplane | Crossplane Workspaces | Provider type directories |
| &emsp;&emsp;&emsp;/tf-workspace | TF provider workspaces | Sub-directory per customer instance (e.g. dev/prod/qa)| 
