Role Name
=========

Transforms raw block storage into a working mounted partition.

Requirements
------------

TODO

Role Variables
--------------

* bd_install: true
* bd_block_device: /dev/xvdf
* bd_file_system: xfs
* bd_mount_point: /var/lib/mysql
* bd_label: MYSQL

Dependencies
------------

* kurron.base

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.block-device,  bd_block_device: /dev/sdb, bd_mount_point: /mnt/data, bd_label: MYSQL }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
