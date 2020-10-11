Role Name
=========

Ansible playbook to install docker-ce and docker compose in Debian

Requirements
------------

Any system running this playbook should have ansible installed. Check [ansible installation docs](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) for platform specific instructions.

Role Variables
--------------

All role specific variables that can be changed are in defaults/main.yml

| Key                        | Value                                        | Description                                  |
|----------------------------|----------------------------------------------|----------------------------------------------|
| docker_compose_version     | 1.24.4                                       | install a sepcific version of docker compose |
| docker_compose_install_dir | /usr/local/bin                               | location for docker_compose binary to live   |

Run the Playbook
----------------

Have all your hosts in a [host-file](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html).

ansible-playbook -h hosts ansible-docker.yml -kK

License
-------

BSD
