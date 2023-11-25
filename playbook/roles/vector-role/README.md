Vector-role
=========

The role installs and configures the `vector` application.   
Supported and tested operating system `Centos 7`.

Role Variables
--------------

- `clickhouse_url` - ip-address API `clickhouse` 
- `vector_version` - version of the application being installed

Example Playbook
----------------

```yml

- hosts: vector
  tags: [vector]
  roles:
    - vector-role
```

License
-------

MIT

---

