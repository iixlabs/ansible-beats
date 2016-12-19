Ansible Beats
===============


Ansible role for installing different elastic beats on your server

Supported beats
* dockbeat
* packetbeat
* pingbeat

Requirements
------------

Install [Ansible](http://www.ansible.com) on your computer, refer to the official [documentation](http://docs.ansible.com/intro_installation.html) for more details.

Installation
------------

`ansible-galaxy install https://github.com/iixlabs/ansible-beats`

Role Variables
--------------

All variables are defined in the file **defaults/main.yml**. 
They will enable the different beat that you want to install and the versions to use

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
    beats_elasticsearch_host: localhost
    beats_elasticsearch_port: 9200
  roles:
    - beats
```

License
-------

Apache 2.0
