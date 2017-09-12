Symfony 2
=========

Requirements
------------

Example Playbook
----------------

    - hosts: backend
      roles:
        - symfony2

      vars:
        symfony_project_root: /var/www/my_project
        symfony_project_name: sportfaction
        symfony_project_composer_path: /var/www/my_project/shared/composer.phar
        symfony_project_repo: git@ip:my_project.git
        symfony_project_env: prod

        symfony_project_post_folder_creation_tasks: "{{playbook_dir}}/roles/symfony2/hooks/post_folder_creation.yml"

        symfony_project_console_opts: '--no-debug'

        symfony_project_release: ~
        symfony_project_branch: "master"
        symfony_project_php_path: php
        symfony_project_keep_releases: 5
        symfony_project_git_clone_depth: 1

        symfony_project_manage_composer: True
        symfony_project_composer_opts: '--no-dev --optimize-autoloader --no-interaction'

        symfony_project_parameters_file: parameters_prod.yml

        symfony_project_enable_post_cmd: True
        symfony_project_fire_schema_update: True
        symfony_project_fire_migrations: True