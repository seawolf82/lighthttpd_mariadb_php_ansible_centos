# lighttpd_mariadb_php_ansible_centos8

This ansible script install on remote machine lighttpd+mariadb+php

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.9 Ansible version

To install run:

ansible-playbook -vv -i hosts site.yaml

To uninstall run:

ansible-playbook -vv -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade package php lighttpd mariadb

For example, to launch only task regarding upgrade os, run:

ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
