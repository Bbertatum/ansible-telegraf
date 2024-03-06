Ansible Telegraf
=========

This role installs and configure telegraf to send data to localhost influxDB.

Requirements
------------

* Debian
* CentOS

A defined and configured influxDB server

Role Variables
--------------

influxdb_yum_url: https://repos.influxdata.com/rhel/$releasever/$basearch/stable
influxdb_yum_key: https://repos.influxdata.com/influxdata-archive_compat.key
influxdb_apt_key: https://repos.influxdata.com/influxdata-archive_compat.key
influxdb_server_ip: localhost


Example Playbook
----------------

```
- hosts: servers
  roles:
    - telegraf
```

License
-------

MIT

Author Information
------------------

Bertrand Cebador
