watchman
========

Installs Watchman

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name                       | Default                               | Description                                 |
|----------------------------|---------------------------------------|---------------------------------------------|
| watchman_repository_url    | https://github.com/facebook/watchman  | URL of watchman repository                  |
| watchman_version           | v4.1.0                                | Version of watchman to install              |

Example Playbook
----------------

Install Watchman
```
- hosts: all
  roles:
    - { role: dpursehouse.watchman }
```

Install Watchman specifying version
```
- hosts: all
  roles:
    - { role: dpursehouse.watchman, watchman_version: ba9f239f69287a553ca93af76a27484d83693563 }
```

License
-------

MIT

Author Information
------------------

David Pursehouse
