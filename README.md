dudefellah.zookeeper
=========

This role downloads, installs and configures Apache Zookeeper on a node.

Requirements
------------

This role won't install the Java Runtime Environment (JRE) for you, so this must
be done first. There are many ways of doing this including the use of other
roles, or just using your system's package manager. That part is up to you.

Role Variables
--------------

All variables are listed and commented in [defaults/main.yml](defaults/main.yml).
Please refer there for more information.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: zookeeper
      tasks:
        - include_role:
            name: dudefellah.zookeeper
          vars:
            zookeeper_data_dir: /var/lib/zookeeper/data

License
-------

GPLv2+

Author Information
------------------

Dan - github.com/dudefellah
