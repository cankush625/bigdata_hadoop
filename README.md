# Ansible Collection - cankush625.bigdata_hadoop

This collection contains the roles for configuring the Hadoop for solving bigdata use cases.

Pre-requisits:
==============

The managed nodes should contain `jdk-8u171-x64.rpm` and `hadoop-1.2.1-1.x86_64.rpm` packages at the $HOME (home directory of the ansible ssh user). Java and Hadoop should not be installed in the managed nodes already.

Roles
=====

mapred_job_tracker
-----------

This role is created for configuring MapReduce job tracker. You can find more information about it in the roles/mapred_job_tracker/README.md file.

mapred_task_tracker
----------

This role is created for configuring MapReduce task tracker. You can find more information about it in the roles/mapred_task_tracker/README.md file.

Installation and Usage
======================

Download and install this collection using following command<br>

`ansible-galaxy collection install cankush625.bigdata_hadoop`

Example playbook for using mapred_job_tracker role from this collection

    - hosts: jobtracker
      collections:
        - cankush625.bigdata_hadoop

      roles:
        - role: mapred_job_tracker

Example playbook for using mapred_task_tracker role from this collection

    - hosts: tasktracker
      collections:
        - cankush625.bigdata_hadoop

      roles:
        - role: mapred_task_tracker
          job_tracker_ip: JOB_TRACKER_PUBLIC_IP

Tested on
=========

This role is tested on following OS distributions: <br>
- Amazon Linux 2 <br>
- RedHat Enterprise Linux v8

Contribution
============

If you find any bug or want to improve this collection, then find the source code for this collection [here](https://github.com/cankush625/bigdata_hadoop). Create an issue or open up a pull request and I will consider merging it, if it does what this collection is intended for.

License
=======

MIT

Author
======

[Ankush Chavan](https://www.linkedin.com/in/ankushchavan)