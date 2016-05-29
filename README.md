watanany.rbenv
=========

This role install rbenv in system-wide by creating `rbenv` group and adding user(rbenv_user) to the group.

The member in rbenv group can use rbenv without sudo.

After installation with ansible, you need to login again to enable unix group.


Requirements
------------

git

Role Variables
--------------

rbenv_user: who is added `rbenv` group (default is /usr/local/rbenv)

rbenv_root: where rbenv will be installed (default is root)

Dependencies
------------

Nothing

Example Playbook
----------------

    - hosts: localhost
      roles:
         - { role: watanany.rbenv, rbenv_user: vagrant }

License
-------

BSD

Author Information
------------------

https://github.com/watanany
