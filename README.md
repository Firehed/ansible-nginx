Nginx
=====

Installs and configures Nginx

Requirements
------------

Only CentOS is supported at this time. Developed and tested on CentOS7, but it will probably work on any OS that uses Yum.

Role Variables
--------------

    nginx_user: nginx
    nginx_group: nginx

Dependencies
------------

The `Firehed.nginx-vhost` role is strongly recommended, as this role will not actually configure any virtual hosts, just Nginx itself.


Example Playbook
----------------
    - hosts: servers
      roles:
         - role: Firehed.nginx
           nginx_user: nginx
           nginx_group: nginx

License
-------

MIT