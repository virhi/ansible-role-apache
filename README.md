Apache
=========

Easy instal and configuration of apache.

Requirements
------------
none

Role Variables
--------------

1. `apache_path`: by default: /etc/apache2
1. `apache_envars_template`: by default: envvars.tpl
1. `ws_vhost_path`: by default: /etc/apache2/sites-available
1. `ws_vhost_path`: by default: /etc/apache2/sites-available

1. `apache24_template`: by default: vhost24.conf.tpl
1. `apache22_template`: by default: vhost22.conf.tpl

1. `apache_run_user`: by default: www-data
1. `apache_run_group`: by default: www-data

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
       - {
        role: virhi.apache,
        apache24_template: template.tpl,
        apache22_template: template.tpl,
        ws_vhost_env: dev,
        servername: dev.vansible.local,
        doc_root: /vagrant/project/web,
        directory_index: app_dev.php
      }

License
-------

MIT

Author Information
------------------

http://github.com/virhi
