Role jj0cker.repo_bareos
=========

Install the bareos repository for RHEL/CentOS, Debian.

Requirements
------------

None.

Role Variables
--------------

  repo_bareos_version: 18.2
  repo_bareos_enabled: true
  repo_bareos_gpgcheck: true


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: j0cker.bareos_repo }

License
-------

MIT / BSD

Author Information
------------------

Created by jj0cker.
