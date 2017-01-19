grub-config
===========

[![Build Status](https://travis-ci.org/cognifloyd/ansible-role-grub-config.svg?branch=master)](https://travis-ci.org/cognifloyd/ansible-role-grub-config)

Manage grub2 configuration on RHEL/CentOS

Requirements
------------

Grub is expected to be installed and working on the guest.

Role Variables
--------------

Values are changed in the file specified with `grub_input_config`
(which defaults to `/etc/defaults/grub`). Currently the only value that will be changed is `grub_timeout`.

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
         - src: cognifloyd.grub-config
           grub_timeout: 1

License
-------

MIT

Author Information
------------------

By Jacob Floyd (@cognifloyd) while working for Theatro Labs, Inc. (theatro.com).
