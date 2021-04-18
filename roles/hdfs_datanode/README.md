hdfs_datanode
=============

Ansible role for configuring HDFS datanode.

Requirements
------------

OS: Amazon Linux 2, RHEL8 <br>
CPU: 1 Cores <br>
RAM: 1GiB

Role Variables
--------------

| Variable                | Required | Default |Example Variable                         |
|-------------------------|----------|---------|-----------------------------------------|
| data_dir                | yes      |         | data_dir: /data                         |
| name_ip                 | yes      |         | name_ip: 192.168.43.21                  |

Dependencies
------------

No any dependency

Example Playbook
----------------

The example playbook below will show how to use this role:

    - hosts: datanode
      roles:
        - role: hdfs_datanode
          data_dir: DATANODE_DIRECTORY
          name_ip: NAMENODE_IP

License
-------

MIT

Author Information
------------------

[Ankush Chavan](https://www.linkedin.com/in/ankushchavan)
