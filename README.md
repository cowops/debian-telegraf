Debian-Telegraf
===============

Time-Series Data Collector

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

telegraf:
  version: 1.2.0
  database: telegraf
  url: http://localhost:8086

Dependencies
------------

  - cowops.debian-influxdb

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-telegraf, telegraf.version: 1.2.0, telegraf.database: telegraf, telegraf.url: 'http://localhost:8086' }

Tasks
-----

  - Install [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/)

License
-------

BSD
