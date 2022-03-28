# Ansible Role: pve_vm_state

### Homelab Virtual Environment project

Updates the state of virtual machine guests (eg stopped, restarted) on a ProxmoxVE host

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see ```defaults/main.yml```)
```shell
proxmox_host: 192.168.0.1
proxmox_user: root@pam
proxmox_password: password
vm_guest:
  - name: vm01
    state: started
  - ...etc...
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: localhost
      roles:
        - pve_vm_state
```

## License

GNU General Public Licence v3.0

## Author Information

This role was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
