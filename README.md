# README.md
# Ansible Role: v2ray

An Ansible role that install and upgrade v2ray powered by official bash scripts

## Requirements

add your `config.json` to `files`  dir with name : `config.json`

## Role Variables

none

## Dependencies

none

## Example Playbook

```
# use this role with root
- hosts: proxy
  roles:
    - jinmiaoluo.v2ray
```

```
# use this role with user non-root
- hosts: proxy
  roles:
    - { role: jinmiaoluo.v2ray, become: yes }
```

## License

BSD