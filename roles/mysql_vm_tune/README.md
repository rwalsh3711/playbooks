Role Name
=========

Tune MySQL VM's by modifying vm.swappiness to 0 and changing I/O scheduler to "noop"

Requirements
------------

To be used on MySQL Linux VM's running RHEL => 6

Role Variables
--------------

sched_type should be set to "noop"
desired_vm_swappiness should be set to "0"

Dependencies
------------

No dependancies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: mysql_vm_tune, sched_type: noop, desired_vm_swappiness: 0 }

License
-------

BSD

Author Information
------------------

Rick Walsh
richard_walsh@optum.com
