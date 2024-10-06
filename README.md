Initialize server for Ansible
=========

[![CI](https://github.com/dtoch56/ansible-role-initialize-server-for-ansible/workflows/CI/badge.svg?event=push)](https://github.com/dtoch56/ansible-role-ssh/actions?query=workflow%3ACI)
[![Release](https://github.com/dtoch56/ansible-role-initialize-server-for-ansible/workflows/Release/badge.svg?event=push)](https://github.com/dtoch56/ansible-role-ssh/actions?query=workflow%3ARelease)
[![Role](https://img.shields.io/ansible/role/53355)](https://galaxy.ansible.com/dtoch56/ssh)
[![Downloads](https://img.shields.io/badge/dynamic/json?color=blueviolet&label=Galaxy%20Downloads&query=%24.download_count&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Froles%2F53355%2F%3Fformat%3Djson)](https://galaxy.ansible.com/dtoch56/ssh)


Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Variable                     | Description            | Default     |
|------------------------------|:-----------------------|:------------|
| ansible_user                 |                        |             |
| ansible_user.home            | Home directory         | /home/ansbl |
| ansible_user.home.user.name  | User name              | ansbl       |
| ansible_user.home.user.id    | User ID (UID)          | 990         |
| ansible_user.home.group.name | Primary group name     | ansbl       |
| ansible_user.home.group.id   | Primary group id (GID) | 990         |

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: dtoch56.initialize_server_for_ansible }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2024 by Max Mudrichenko.

Development
------------------

    pip install pipenv
    pipenv install
