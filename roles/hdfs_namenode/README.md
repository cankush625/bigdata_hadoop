hdfs_namenode
=============

Ansible role for configuring HDFS namenode.

Requirements
------------

OS: Amazon Linux 2, RHEL8 <br>
CPU: 1 Cores <br>
RAM: 1GiB

Role Variables
--------------

| Variable                | Required | Default |Example Variable                         |
|-------------------------|----------|---------|-----------------------------------------|
| name_dir                | yes      |         | name_dir: /name                         |
| name_ip                 | yes      |         | name_ip: 192.168.43.21                  |

Dependencies
------------

No any dependency

Example Playbook
----------------

The example playbook below will show how to use this role:

    - hosts: namenode
      roles:
        - role: hdfs_namenode
          name_dir: NAMENODE_DIRECTORY
          name_ip: NAMENODE_IP

License
-------

MIT

Author Information
------------------

[Ankush Chavan](https://www.linkedin.com/in/ankushchavan)
