# Proxmox New VM Guest From Template
![proxmox](https://img.shields.io/badge/-ProxmoxVE-black?style=flat&logo=proxmox)
[![playbook](https://img.shields.io/badge/Ansible%20Playbook-grey?stype=flat&logo=ansible&logoColor=EE0000)](site.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/lpwoodhouse/proxmox_new_vm)
![GitHub repo file count](https://img.shields.io/github/directory-file-count/lpwoodhouse/proxmox_new_vm)
![GitHub top language](https://img.shields.io/github/languages/top/lpwoodhouse/proxmox_new_vm)
[![GitHub](https://img.shields.io/github/license/lpwoodhouse/proxmox_new_vm)](LICENSE)
## Purpose

This play is for creating new virtual machine guest(s) from a clone on a ProxmoxVE host

## Requirements

community.general

## Role Variables

Default role variables for the pve_new_vm role are listed below (see ```defaults/main.yml```)
```shell
# pve host credentials
proxmox_host: <pve_host_ip_addr>
proxmox_user: <root@pam>
proxmox_password: <password>
proxmox_node: <pve_node_name>

# new vm variables
vm_id: <100>
vm_name: <new_vm_name>
vm_clone: <template_name>
vm_storage: <storage_name>
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: localhost
      roles:
        - pve_new_vm
```

## Author Information

This playbook was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
