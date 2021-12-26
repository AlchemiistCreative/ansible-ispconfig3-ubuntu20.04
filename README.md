ISPConfig 3 installation: Ubuntu 20.04
=========

This role is based on the tutorial from howtoforge.com [The Perfect Server](https://www.howtoforge.com/tutorial/perfect-server-ubuntu-20.04-with-apache-php-myqsl-pureftpd-bind-postfix-doveot-and-ispconfig/)

Requirements
------------

OS: Ubuntu 20.04

An user in sudoers group

Role Variables
--------------

Every variables located in defaults/main.yml should be modified to fit for your needs.

Any password should be vaulted for security reasons.

Example Playbook
----------------

Example configuration of your playbook:

      hosts: ispconfig_host
      roles:
      - role: ispconfig3
        admin_email: email@example.com
        mail_fqdn: mail.example.com
        ispconfig_hostname: server1.example.com
        hostname_needed: true
        user_ispconfig: admin_ispconfig
  

License
-------

BSD


