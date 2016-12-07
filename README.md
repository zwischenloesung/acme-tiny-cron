Role Name
=========

Requirements
------------

* Ansible >2.0
* On target host
 * Generic UNIX with FHS
 * Python2/3
 * Cron
 * Running webserver with ^/.well-known/acme-challenge/ directory accessible (hardcoded in acme-tiny script..)
 * The webserver must serve HTTP, even for consequent certificates (not just HTTPS; requirement of acme-tiny/let's-encrypt)
 * Resolve all names in the cert to localhost or the local-IP

Role Variables
--------------

* app\_\_acme\_\_tiny\_\_user - optional, default='acme'
* app\_\_acme\_\_tiny\_\_config\_dir - optional, default='/etc/ssl/acme-tiny'
* app\_\_acme\_\_tiny\_\_account\_key - optional, auto
* app\_\_acme\_\_tiny\_\_challenge\_dir - optional, default='/var/www/acme-challenge'
* app\_\_acme\_\_tiny\_\_domain - optional, default='example.com'
* app\_\_acme\_\_tiny\_\_cert\_name - optional, auto
* app\_\_acme\_\_tiny\_\_cert\_dir - optional, auto
* app\_\_acme\_\_tiny\_\_request - optional, auto

Dependencies
------------


Example Playbook
----------------

License
-------

GPLv3

Author Information
------------------

