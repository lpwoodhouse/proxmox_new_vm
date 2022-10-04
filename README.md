# Ansible Play: proxmox_new_vm

## Purpose

This play is for createing new virtual machine guest(s) from a clone on a ProxmoxVE host

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

## License

MIT

## Author Information

This role was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
