# Docker
This role installs and configures a docker server.

## Requirements
Tested on centos 7, centos 8 and RockyLinux 8.4

## Role Variables

## Example Playbook

The following sample playbook will install docker on the target host and also ensure that ansible is added to the docker user group. 
docker-compose will also be installed. 

```
- hosts: harbor.lab.jnvilo.com
  become: true
  remote_user: ansible
  gather_facts: no
  roles:
    - docker
```
