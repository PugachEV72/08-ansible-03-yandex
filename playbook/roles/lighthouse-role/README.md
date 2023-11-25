Lighthouse-role
=========

The role installs and configures the `lighthouse` application.   
Supported and tested operating system `Centos 7`.

Role Variables
--------------

- `lighthouse_home_dir` - home directory `lighthouse` 
- `nginx_config_dir` - directory of the `nginx` config location 

```yml

lighthouse_home_dir: "/usr/share/nginx/html/lighthouse"
nginx_config_dir: "/etc/nginx"

```

Example Playbook
----------------

```yml

- hosts: lighthouse
  tags: [lighthouse]
  roles:
    - lighthouse-role
```

License
-------

MIT

