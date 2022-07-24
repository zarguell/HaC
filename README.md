# HaC
HomeLab As Code: Infrastucture as Code configurations for a Proxmox managed bare metal k3s homelab. 

# Design Goals

1. Configure Proxmox image & template creation (Packer)
2. Configure & deploy packer created VMs (Ansible/Terraform)
3. Deploy services to k3s cluster (Helm)

# Pre-Requisites

- Host with Packer
  - Packer host -> Access to Proxmox Host
  - Proxmox host -> Access to Packer host (to download kickstart file)
- Pre-Downloaded Linux ISOs
  - While I wanted to automate the download of the ISO, it is not efficient to download full DVD ISOs to packer host, then upload to Proxmox
  - My preference: setup an NFS share for all proxmox host ISOs and download all ISOs centrally
