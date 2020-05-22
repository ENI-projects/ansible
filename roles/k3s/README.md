k3s
=========

A simple role to install a k3s cluster using rancher's install script.

Requirements
------------

The role is not idempotent so you'll need to start from fresh machines.

Role Variables
--------------

* k3s_version: the version of k3s you want to install
* master_ip: the ip of the master node for the workers to connect to it

Dependencies
------------

None.

Example Playbook
----------------

- name: Installing k3s cluster
  hosts: k3s
  roles:
    - k3s

License
-------

MIT

Author Information
------------------

Matthieu Chevreux, SRE @RCA-logiciels, living in Nantes, France.
