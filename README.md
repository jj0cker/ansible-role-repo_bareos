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
  repo_bareos_filename: bareos
  repo_bareos_release: experimental/nightly
  repo_bareos_os_version: "{{ ansible_distribution_major_version }}"
  __repo_bareos_release: release
  repo_bareos_distro: 


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: j0cker.bareos_repo }

TODO
----

Add Ubuntu and maybe Fedora.

License
-------

MIT / BSD

Author Information
------------------

Created by jj0cker.
