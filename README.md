Flush Handlers
==============

Sometimes you need to force handlers from a previous role to run before executing a subsequent role.

This role simply flushes all handlers.


Example playbook
----------------

    - hosts: localhost
      roles:
      - role: role1
      - role: flush_handlers
      - role: role2-depends-on-role1


Author Information
------------------

ome-devel@lists.openmicroscopy.org.uk
