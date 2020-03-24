Junos Policy Configuration
=========

This role will configure junos policies
 
Requirements
------------
ncclient


Role Variables
--------------
* ecmp: True|False
* policies: List
  * name: String
  * terms: List
    * id: String
    * froms: List
      * type: String
      * data: String
    * thens: List
      * type: String ('terminate'|'community')
      * type_action: String ('add'|'remove')
      * data: String
      * terminating_action: String ('accept'|'reject'|'discard')
* communities: List
  * name: String
  * id: String
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
