mail_aliases
============

Configures email aliases.

Role Variables
--------------

 * mail_aliases: []

    Specifies a list of email aliases that should be configured. See example below.

 * mail_aliases_to_remove: []

    Specifies a list of email aliases that should be removed. See example below.

Example Playbook
----------------

    - hosts: servers
      vars:
        mail_aliases:
          - { name: root, alias: sysadmin@somewhere.com }
          - { name: joe, alias: jsmith@gmail.com }
        mail_aliases_to_remove:
          - { name: bob }
      roles:
        - mail_aliases

License
-------

BSD

Author Information
------------------

Adam Herzog <adam@adamherzog.com>
