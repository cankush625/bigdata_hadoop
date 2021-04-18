mapred_task_tracker
===================

Ansible role for configuring MapReduce Task Tracker.

Requirements
------------

OS: Amazon Linux 2, RHEL8 <br>
CPU: 1 Cores <br>
RAM: 1GiB

Role Variables
--------------

| Variable                | Required | Default |Example Variable                         |
|-------------------------|----------|---------|-----------------------------------------|
| job_tracker_ip          | yes      |         | job_tracker_ip: 192.168.43.21           |

Dependencies
------------

No any dependency

Example Playbook
----------------

The example playbook below will show how to use this role:

    - hosts: tasktracker
      roles:
        - role: mapred_task_tracker
          job_tracker_ip: JOB_TRACKER_PUBLIC_IP

License
-------

MIT

Author Information
------------------

[Ankush Chavan](https://www.linkedin.com/in/ankushchavan)
