Grub-config
===========

Manage grub2 configuration on RHEL/CentOS

Requirements
------------

Grub is expected to be installed and working on the guest.

Role Variables
--------------

`grub_config` is a dictionary of values to change in the file specified with `grub_input_config`
(which defaults to `/etc/defaults/grub`). Currently the only value that will be changed is timeout.

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
         - src: cognifloyd.grub
           grub_config.timeout: 1

License
-------

MIT

Author Information
------------------

By Jacob Floyd (@cognifloyd) while working for Theatro Labs, Inc. (theatro.com).
