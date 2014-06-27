Role Name
========

Ansible role that installs ElkarBackup on Debian/Ubuntu variants. ElkarBackup is a free open source backup solution. More info: http://elkarbackup.org

Features:
 * Installation of ElkarBackup and it's dependencies
 * Basic configuration

To do:
 * _version_ variable to choose between _stable_ or _dev_

Requirements & Dependencies
------------

__Important__: MySQL server needed.

You can install it, for instance, with the package __Ansibles.mysql__


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
