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

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD-3-Clause

Author Information
------------------

This role was created in 2021 by K. Scott Tripp
