Symfony 2
=========

This roles helps to install Symfony2 on Ubuntu

Requirements
------------

This role requires Ansible 1.4 or higher, and platform requirements are listed
in the metadata file.

Example Playbook
----------------

    - hosts: localhost
      roles:
        - ansible-role-symfony2

      vars:
        symfony_dir: "/var/www/"
        repo_git: "git@ip:repo.git"
        env: "prod"
        branch: "master"

Dependencies
------------

None

License
-------

BSD
