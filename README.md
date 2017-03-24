NFS server Ansible role
======================

Installs & configures nfs server & exports on Ubuntu 16.04+

Requirements
------------

None

Role Variables
--------------

`nfs_server_export_directories`: yaml structure containing an export line to add or change

Example
-------

```
nfs_server_export_directories:
  - path: "/tmp"
    clients:
      - "localhost(rw,no_root_squash)"
      - "foo.dev(rw,no_root_squash)"
  - path: "/data/backups"
    clients:
      - "server1(rw,no_root_squash)"
      - "server2(rw,no_root_squash)"
```

License
-------

MIT

Author Information
------------------

@leucos

