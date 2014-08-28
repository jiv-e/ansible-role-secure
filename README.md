Ansible role - Secure
========

This role does a basic hardening for an Ubuntu server.

The role is based on Linode documentation. https://library.linode.com/securing-your-server

Disclaimer
----------
Even if this script does some security related configuration I don't guarantee
that your server will be secure after running it. You have ensure this yourself.

Provides
--------
* Configuration described on https://library.linode.com/securing-your-server
* Logwatch monitoring
* Ansible inventory file template (./hosts)
* Empty SSH related files for adding your keys
  - authorized_keys
  - id_rsa
  - id_rsa.pub
  - known_hosts
* Editable settings including (./group_vars/servers)
  - System user name
  - Password for the user
  - Admin email
  - SSH port
  - Fail2Ban - maxretry, bantime

Requirements
------------
* Ansible (tested on 1.6)
  - http://docs.ansible.com/intro_installation.html
* Ubuntu server (tested on vanilla 12.04 LTS)

You have to run this role as root.

Role Variables
--------------

TODO

Dependencies
------------

None.

Example Playbook
-------------------------

TODO

License
-------

MIT/BSD
