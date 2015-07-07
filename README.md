Ansible Uchiwa Role
==================
[![Build Status](https://travis-ci.org/michaelrigart/ansible-role-users.svg?branch=master)](https://travis-ci.org/michaelrigart/ansible-role-users)

An ansible role for installing the Uchiwa dashboard for the Sensu monitor framework.
Visit the [Uchiwa website](https://uchiwa.io) for more info

Role Variables
--------------

```yaml
uchiwa_service_state: indicates the service state; Allowed setting: started, stopped
uchiwa_service_enabled: indicates if service needs to be enabled on boot; Allowed settings: yes, no
uchiwa_ppa_key: location of the public ppa key for the repository
uchiwa_ppa_key_id: the repository key id
uchiwa_ppa_repo: the ppa repo location
uchiwa_conf: dictionary containing the Uchiwa configuration. See the defaults for more information
```


Example Playbook
-------------------------

```yaml
- hosts: servers
  roles:
     - { role: MichaelRigart.uchiwa, sudo: Yes }
```
License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>