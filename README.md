Role Name
=========

A role to configure flow-tools package.

Requirements
------------

None.

Role Variables
--------------

  flow_tools_collectors:
    - name: example-1
      flows_dir: /flow/example-1
      port: 558 # default 2055
      listen_address: 127.0.0.1 # default 0 (all)
      remote_address: 192.0.2.1 # default 0 (all)
      rotate_interval: 15
      options:
        expire_size: 300G
	nesting_level: 3
	compression: 1


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: flow-tools

License
-------

CC0-1.0

Author Information
------------------

nikty
