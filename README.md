Docker convenience script
[![Build Status](https://travis-ci.com/mivek/ansible-role-docker-convenience-script.svg?token=Nxd1CoxuZDnwzK6Yq6sV&branch=master)](https://travis-ci.com/mivek/ansible-role-docker-convenience-script)
=========

This role installs [Docker](https://www.docker.com/) via convenience script.
This can be run on Raspberry Pi. 

Requirements
------------

None.
Required packages are installed by the role.

Role Variables
--------------

```(yaml)
install_test_version: false   # Whether to install the test version of Docker

docker_users: []              # Users allowed to use docker

install_compose: true         # Whether to install docker compose.
```

Dependencies
------------

None.

Example Playbook
----------------

```(yaml)
- hosts: all
  tasks:
    - name: "Include docker_convenience_script"
      include_role:
        name: "docker_convenience_script"
      vars:
        install_test_version: true
```


License
-------

MIT

