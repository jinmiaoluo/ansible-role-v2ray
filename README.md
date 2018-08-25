# README.md

[![Join the chat at https://gitter.im/ansible-role-v2ray/Lobby](https://badges.gitter.im/ansible-role-v2ray/Lobby.svg)](https://gitter.im/ansible-role-v2ray/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# Ansible Role: v2ray

An Ansible role that install and upgrade v2ray powered by official bash scripts

## Requirements

add your `config.json` to `files`  dir with name : `config.json` or change `v2ray_config_file_path` value to where your config is. 


## Role Variables

```
v2ray_config_file_path: '{{ role_path }}/files/config.json'
```

## Dependencies

none

## Example Playbook

use this role with root
```
- hosts: <your-host>
  roles:
    - jinmiaoluo.v2ray
```

use this role with account non-root
```
- hosts: <your-host>
  roles:
    - { role: jinmiaoluo.v2ray, become: yes }
```
if your account need pass to become root, for example `sudo` command. use `ansible-playbook <your-playbook> --ask-become-pass`

## License

BSD