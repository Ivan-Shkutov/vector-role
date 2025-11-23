# Role Name


Действия для установки Vector:

- установка vector

- создание systemd unit vector

- ностройка vector на передачу данных в clickhouse

------------

# Requirements

------------

# Role Variables

       clickhouse_user: user
       clickhouse_password: 1234

Конфигурация содержится в vars/main.yml

------------

# Dependencies


В inventory добавляем название хоста clickhouse

       endpoint: http://{{ hostvars['clickhouse'].ansible_host }}:8123

------------

# Example Playbook


       - hosts: vector
         roles:
          - role: vector-role

------------

# License

MIT

------------

# Author Information

Ivan Shkutov

------------
