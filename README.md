File retention
=========

An ansible role to delete oldest files/path in a defined path

Requirements
------------

Need ansible 2+ and cron on the target host.

Role Variables
--------------

```yaml
file-retention_path = '/data/db/backups'
file-retention_days = 30;
file-retention_user = 'www';
```

Dependencies
------------

There is no dependency

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: SimpliField.file-retention
    file-retention_path: '/data/db/backups'
    file-retention_days: 30
    file-retention_user: 'www'
```

License
-------

BSD
