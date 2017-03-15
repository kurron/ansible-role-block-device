Role Name
=========

Transforms raw block storage into a mounted file system.  By default,
the device will not be partitioned.  This is useful when having to grow
the file system after expanding a virtual block device.

Requirements
------------

TODO

Role Variables
--------------

* bd_install: true
* bd_block_device: /dev/xvdf
* bd_create_partition: false
* bd_file_system: xfs
* bd_mount_point: /var/lib/mysql
* bd_label: MYSQL
* bd_options: defaults

Dependencies
------------

* kurron.base

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.block-device,  bd_block_device: /dev/sdb, bd_mount_point: /mnt/data, bd_label: MYSQL, bd_options: noatime }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
