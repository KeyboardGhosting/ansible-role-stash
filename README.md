Ansible Role: stash
=========

Installs Stash on Linux machines.

Requirements
------------

Permission to:
  - Create or modify users/groups
  - Create or modify required directories

Role Variables
--------------
A list of variables is listed below along with their default values.

    stash_version: '0.18.0'

The version of Stash to download and install.

    stash_user: 'stash'
    stash_group: 'stash'

The user and group that will be created and Stash will run under.

    stash_daemon: 'stash'

The name of the service used to control the Stash process.

    stash_bin_dir: '/opt/stash'

Set to the target directory for the Stash binary.

    stash_data_dir: '/var/opt/stash'

The directory where data for Stash will be stored.

    stash_config_dir: '/etc/opt/stash'

The directory where configs for Stash will be stored.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: keyboardghosting.stash
           become: yes

License
-------

MIT / BSD

Author Information
------------------

This role was created by KeyboardGhosting.
