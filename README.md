# Lighthouse Role


## Description

Deploy LightHouse using Ansible.

## Requirements

- Ansible >= 2.10 (It might work on previous versions, but we cannot guarantee it)

- ## Role Variables

- All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |  
| -------------- | ------------- | -----------------------------------|  
| `user` | root | User in /etc/nginx/nginx.conf file |   

## Example Playbook

```yaml
---
- hosts: all
  roles:
  - lighthouse
  vars:
    user: lighthouse
```