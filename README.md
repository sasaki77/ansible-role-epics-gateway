# Ansible Role: EPICS Gateway

Installs EPICS Gateway on RHEL/CentOS.

## Requirements

- ansible >= 2.3

## Role Variables
Refer to `defaults/main.yml` in detail.
```
gateway_extension:
  url: "https://github.com/epics-extensions/ca-gateway/archive/R2-0-6-0.tar.gz"
  unarchived_name: "ca-gateway-R2-0-6-0"
  release: true
```

## Dependencies

- [ansible-role-epics-base](https://github.com/sasaki77/ansible-role-epics-base)

## Example Playbook
```
- hosts: epics-base
  roles:
    - role: ansible-role-epics-base
    - role: ansible-role-epics-gateway
```

## License

None.

## Author Information

This role was created by Shinya Sasaki.
