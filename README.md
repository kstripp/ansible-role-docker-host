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

### Required variables:

    docker_compose_template: ''

The local path to the compose file for this server.  This file will be installed to /opt/services

### Optional variables:

    service_data_dir: ''

location for persistance data
    
    docker_service_config_file_source: ''
    docker_service_config_file_dest: ''

Additional configration files are specified with `docker_service_config_files` and `docker_service_config_dir`.
`docker_service_config_files` is the local path to the top level of these files.
`docker_service_config_dir` is top level destination path for installing on the server.
`_source` and `_dest` follow the rsync path naming conventions
Note: `docker_service_config_dir` is required when `docker_service_config_files` is defined.

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
        - docker_service_config_file_source: files/etc/
        - docker_service_config_file_dest: /etc

License
-------

BSD-3-Clause

Author Information
------------------

This role was created in 2021 by K. Scott Tripp
