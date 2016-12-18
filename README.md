[![Build Status](https://travis-ci.org/dougbtv/kpm-install.svg?branch=master)](https://travis-ci.org/dougbtv/kpm-install)

kpm-install
===========

This role installs [kpm](https://github.com/coreos/kpm) on CentOS 7 systems.

Requirements
------------

Should be a CentOS 7 system or greater. (Tested only on CentOS 7.3)

Role Variables
--------------

Found in `vars/main.yml`

- `kpm_version`: Defaults to (and only tested with) v0.21.2
- `kpm_jsonnet_url`: URL to jsonnet tarball, currently 0.9.0

Dependencies
------------

This playbook does not require any other ansible galaxy roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: dougbtv.kpm-install }

Testing
-------

You can find a test in `tests/` including a test inventory.

You can run the test like:

```
ansible-playbook -i inventory test.yml
```

License
-------

Apache

Author Information
------------------

The original author is @dougbtv on twitter / github.
