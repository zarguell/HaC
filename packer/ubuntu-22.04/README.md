# Usage

To build, run:

```packer build -var-file=secrets.json ubuntu.json```

Where secrets.json is set as:

```
{
  "proxmox_username": "your pve user",
  "proxmox_password": "your pve password",
  "proxmox_url": "https://pve.example.com:8006/api2/json"
}
```