# HaC
HomeLab As Code: Infrastucture as Code configurations for an r/selfhosted (ProxMox) managed homelab. 

# Design Goals

1. Configure ProxMox image & template creation (Packer)
2. Configure & deploy packer created VMs (Ansible/Terraform)
3. Deploy services to k3s cluster (Helm)

# Pre-Requisites

- Host with Packer
  - Packer host -> Access to Proxmox Host
  - Proxmox host -> Access to Packer host (to download kickstart filee)