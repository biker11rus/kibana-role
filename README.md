Kibana role
=========

Роль для установки Kibana на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

  * Поддерживаются только ОС семейств debian и EL.
  * Elasticsearch


Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| kibana_version | "7.14.0" | Параметр, который определяет какой версии kibana будет установленa |
| elasticsearch_host | "localhost" | Параметр, который определяет ip или имя хоста эластика |
| kibana_host | "0.0.0.0" | Параметр, который определяет ip или имя хоста kibana |
| kibana_port | 5601 | Параметр, который определяет порт kibana |


Example Playbook
----------------

    - hosts: all
      roles:
         - { role: kibana-role }

License
-------

ect

Author Information
------------------

Ruslan Khozyainov netology 
