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

The variable **coreos_timezone** is defined in the file **defaults/main.yml**. 
It must be a valid entry from the system as defined in the folder **/usr/share/zoneinfo**.

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
  roles:
    - beats
```

License
-------

Apache 2.0
