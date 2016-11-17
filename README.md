Role Name
=========

Transforms raw block storage into a working mounted partition.

Requirements
------------

TODO

Role Variables
--------------

None.

Dependencies
------------

* kurron.base

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.block-device }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
