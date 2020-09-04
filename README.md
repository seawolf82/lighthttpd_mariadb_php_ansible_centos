# lighthttpd_mariadb_php_ansible_centos8

This ansible script install on remote machine The lighttpd+mariadb+php7.2
To install run:

ansible-playbook -vv -i hosts site.yaml

To uninstall run:

ansible-playbook -vv -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade package php7 lighttpd mariadb

For example, to launch only task regarding upgrade os, run:

ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
