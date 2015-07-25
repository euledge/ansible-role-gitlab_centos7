ansible-role-gitlab_centos7
=========

The role is created for centos7.
- Installs from git.
- Gitlab running by unicorn and nginx as a frontend.
- Uses database is mariadb instead of Postgresql.

Requirements
------------

- CentOS7
- Ruby (MRI) 2.0 or 2.1
- Git
- MySQL or MariaDB
- Redis (installed by this role)
- nginx

Role Variables
--------------

The role uses the following variables, that you can also override:

* `gitlab_hostname` - override to set the name of the virtual host, also used for email (defaults to `ansible_hostname`)
* `gitlab_branch` - gitlab branch to checkout
* `gitlab_shell_version` - gitlab shell version to checkout
* `gitlab_db_type` - database type to use (mysql by default)
* `gitlab_db_name` - database name (gitlab)
* `gitlab_db_user` - database user (gitlab)
* `gitlab_db_password` - database password (probably should change this, it's some random string now)
* `gitlab_user` - system user that's needed for ssh access
* `gitlab_uwsgi_port` - port used for nginx - uwsgi communucation
* `gitlab_ssh_port` - override if using different port for ssh (22 by default)
* `gitlab_version` - gitlab version to checkout
* `gitlab_shell_version` - gitlab shell version to checkout
* `gitlab_user` - gitlab user (git by default)
* `gitlab_password` - gitlab password
* `gitlab_ssh_port` - gitlab port for ssh (22 by default)
* `gitlab_relative_root` - use sub directory access for gitlab
* `gitlab_hostname` - override to set the name of the virtual host, also used for email
* `gitlab_front_port` - port used for nginx (80 by default)
* `gitlab_backend_port` - port used for unicorn (8080 by default)
* `gitlab_backend_url` - url used for unicorn (http://localhost by default)
* `gitlab_db_name` - database name (gitlab)
* `gitlab_db_user` - database name (gitlab)
* `gitlab_db_password` - database name (gitlab)
* `gitlab_smtp_server` - smtp server hostname for send email by gitlab
* `gitlab_smtp_port` - smtp server port for send email by gitlab

License
-------

Licensed under the MIT License. See the LICENSE file for details.

Author Information
------------------

* Twitter @euleage
* Github https://github.com/euledge 
