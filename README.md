# David Woitzik

System engineer for hybrid cloud. I build Azure infrastructure with Terraform for regulated environments (ISO 27001, NIS2, KRITIS) and run a homelab that is managed the same way: everything in Git, changed through pull requests.

Microsoft Certified: Azure Administrator Associate (AZ-104) · HashiCorp Certified: Terraform Associate

## Terraform modules

Free and MIT licensed, published on the [Terraform Registry](https://registry.terraform.io/namespaces/dwoitzik).

| Module | What it solves |
|--------|----------------|
| [terraform-azurerm-hub-spoke](https://github.com/dwoitzik/terraform-azurerm-hub-spoke) | Hub & Spoke network with Zero-Trust NSGs, central Private DNS linked to every VNet, and a DINE policy bypass so Azure Policy remediation does not show up as drift |
| [terraform-azurerm-firewall-forced-tunneling](https://github.com/dwoitzik/terraform-azurerm-firewall-forced-tunneling) | Azure Firewall forced tunneling without the cycle error, with KMS and Entra ID bypass routes and dynamic IP Groups |
| [terraform-azurerm-acme-cert](https://github.com/dwoitzik/terraform-azurerm-acme-cert) | Let's Encrypt certificates in Key Vault (Acmebot) behind Private Link, default-deny network rules and Managed Identity |
| [terraform-azurerm-openai-rag](https://github.com/dwoitzik/terraform-azurerm-openai-rag) | Network layer for an Azure OpenAI RAG stack: Private Endpoints, Private DNS, RBAC instead of keys |
| [terraform-azurerm-private-aks](https://github.com/dwoitzik/terraform-azurerm-private-aks) | Private AKS: no public API server, no public node IPs, forced-tunneled egress |

## Homelab

[homelab-infrastructure](https://github.com/dwoitzik/homelab-infrastructure): Proxmox, a k3s cluster, MikroTik RouterOS and Raspberry Pi edge nodes, all in Terraform and Ansible. Plans and applies run from pull request comments on a self-hosted GitHub Actions runner, Kubernetes workloads sync through ArgoCD, secrets come from Vault.

## Writing

[woitzik.dev](https://woitzik.dev/blog/) has incident write-ups and how-tos from that setup and from Azure work: what broke, how I found it, and what I changed so it does not happen again.

## Contact

[LinkedIn](https://www.linkedin.com/in/david-woitzik/) · david@woitzik.dev

If the modules or articles saved you time: [GitHub Sponsors](https://github.com/sponsors/dwoitzik) or [Buy Me a Coffee](https://buymeacoffee.com/dwoitzik).
