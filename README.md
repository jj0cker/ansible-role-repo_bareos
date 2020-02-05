Role jj0cker.repo_bareos
=========

Install the bareos repository from download.bareos.org for RHEL/CentOS, Debian.

Requirements
------------

None.

Role Variables
--------------

  repo_bareos_version: 18.2 (Default)
Choose version of the bareos exmaples: latest, 18.2, 17.2, 16.2, 15.2, 14.2, 13.2, 12.4.

  repo_bareos_enabled: true (Default)
  repo_bareos_gpgcheck: true (Default)
This variables is only for RedHat family systems. You can disable/enable repo check or not gpg key.

  repo_bareos_filename: bareos (Default)
Choose repository name for bareos. In Debian family os systems to file name is added postfix .list in RedHat .repo.

  repo_bareos_release: release/{{ repo_bareos_version }} (Default)
Default value of this variable install repository with stable packages of bareos. You can choose for example repository with experimental packages (repo_bareos_release: experimental/nightly). 

  repo_bareos_os_version: "{{ ansible_distribution_major_version }}"
This variable is only for a shorter name.

  __repo_bareos_release: release (Default)
This variable is for internal usage.

  repo_bareos_distro: "{{ ansible_distribution }}"
This variable is for internal usage. This is specific for distribution.


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: jj0cker.bareos_repo }

TODO
----

Add Ubuntu and maybe Fedora.

License
-------

MIT / BSD

Author Information
------------------

Created by jj0cker.
