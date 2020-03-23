Junos Policy Configuration
=========

This role will configure junos policies
 
Requirements
------------
ncclient


Role Variables
--------------
* logical_interfaces
  * mpls
    * state
    * protocol
  * name
  * unit

Dependencies
------------

Example Playbook
----------------

    - hosts: vmx1
      roles:
         - { role: junos_policy_configuration }

License
-------

BSD

Author Information
------------------

Marc Colburn
