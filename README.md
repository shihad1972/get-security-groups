get-security-groups
=========

Giving a list of AWS security group names, return a list of their ID's

Requirements
------------

AWS account and boto on the ansible node.

Role Variables
--------------

  - sec_group_names: A list of Group names. Ensure you are using the 
                     Group Name and not the Name: tag
  - security_group_ids: Returned variable, containting a list of
                     security group ID's
Dependencies
------------

 No other galaxy roles are required to run this role

Example Playbook
----------------

    - hosts: localhost
      vars:
        sec_group_names:
          - My App Group
          - His Web group
      roles:
        - { role: get-security-groups }

License
-------

GPL

Author Information
------------------

Iain M Conochie <iain@shihad.org>
