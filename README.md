Role Name
========

Ansible role that installs ElkarBackup on Debian/Ubuntu variants. ElkarBackup is a free open source backup solution. More info: http://elkarbackup.org

Features:
 * Installation of ElkarBackup and it's dependencies
 * Basic configuration

To do:
 * "version" variable to choose between "stable" and "dev"

Requirements & Dependencies
------------

MySQL server needed, but it doesn't install it to keep it simple.

You can install it with the package _Ansibles.mysql_


Role Variables
--------------

```
#Basic settings
mysql_root_password: 'elkarbackup'
```

Example Playbook
-------------------------

```
    - hosts: all
      roles:
	 - { role: Ansibles.mysql, mysql_root_password: 'elkarbackup' }
         - { role: elkarbackup.ansible, mysql_root_password: 'elkarbackup' }
```


License
-------

BSD

Author Information
------------------

More info: http://elkarbackup.org
