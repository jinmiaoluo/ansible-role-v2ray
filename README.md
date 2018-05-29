# README.md
# Ansible Role: v2ray

An Ansible role that installs v2ray latest on Ubuntu 18.04

## Requirements

add your config.json to role template dir with name : v2ray.j2

## Role Variables

none

## Dependencies

none

## Example Playbook

    - hosts: proxy
      roles:
        - { role: jinmiaoluo.v2ray }

## License

BSD