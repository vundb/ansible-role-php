Ansible Role PHP
======================================

Ansible role to install and configure php on gentoo instances.

Supported Distributions
-----------------------

- Gentoo

Role Variables
--------------

- `php_services`:
Array with services to be restarted after configuration changes.

- `php_version`:
PHP Version to be installed. Supported values are ["5.6", "7.0", "7.1", "7.2"]

- `php_extensions`:
Array with PHP extensions to be installed. Supported values are ["apache2", "fpm"]

- `php_config`:
Array with configuration entries. See [default vars file](defaults/main.yml)

Dependencies
------------

[vundb/ansible-role-portage](https://github.com/vundb/ansible-role-portage)

Example Playbook
----------------
```
- hosts: all
  roles:
    - role: vundb-php
      php_extensions: ["apache2"]
```

License
-------

MIT

Author Information
------------------

- You can find more roles in my GitHub channel [vundb](https://github.com/vundb)
- Follow me on Twitter [@vundb](https://twitter.com/vundb)
