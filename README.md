troykinsella.vagrant
====================

An ansible role for installing HashiCorp Vagrant.

Dependencies
------------

* troykinsella.deb

Role Variables
--------------

* vagrant_version: Optional. The Vagrant version to download. Default: 1.8.3.
* vagrant_architecture: Optional. The target system architecture. Default: x86_64.
* vagrant_package_url: Optional. The URL at which the Vagrant deb package can be downloaded. Default: https://releases.hashicorp.com/vagrant/{{ vagrant_version }}/vagrant_{{ vagrant_version }}_{{ vagrant_architecture }}.deb.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: troykinsella.vagrant

License
-------

MIT
