Ansible Beats
===============


Ansible role for installing different elastic beats on your server

Requirements
------------

Install [Ansible](http://www.ansible.com) on your computer, refer to the official [documentation](http://docs.ansible.com/intro_installation.html) for more details.

Installation
------------

`ansible-galaxy install console.beats`

Role Variables
--------------

The variable **dockbeat_enabled** is defined in the file **defaults/main.yml**. This enables the different beat that you want to install

Dependencies
------------

None

Example Playbook
----------------

```yml
---
- hosts: myhosts
  sudo: true
  vars:
    dockbeat_enabled: true
    dockbeat_elasticsearch_host: localhost
    dockbeat_elasticsearch_port: 9200
  roles:
    - beats
```

License
-------

Apache 2.0
