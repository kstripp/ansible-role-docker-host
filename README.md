Role Name
=========

This role that configures services defined in a docker-compose file.
This is a fairly specific role, tailored to how I use a docker host
in my homelab.

For a more generic docker host role, you may be more interested in 
geerlingguy/docker, 
and possibly IronicBadger/ansible_role_docker_compose_generator 

Requirements
------------

None

Role Variables
--------------

Required variables:

    docker_compose_template: path to the compose file for this server

Optional variables:

    service_data_dir: location for persistance data


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - ansible-role-docker-host
      vars:
        - docker_compose_template: compose_file.yml

License
-------

BSD-3-Clause

Author Information
------------------

This role was created in 2021 by K. Scott Tripp
