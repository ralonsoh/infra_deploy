Infraestructure deployment
==========================
This project allows to deploy a virtualized infraestructure, using virsh. The
ansible script, using the inventory file defined by the user (e.g.
/etc/config_01.yaml), creates the needed XML files to deploy the networks (using
linux brige) and the virtual machines.

In order to define the user and the password, and the management network
configuration, this project uses `cloud-init NoCloud`_.


Requirements
------------
ansible >= 2.6.4


References
==========
.. _`cloud-init NoCloud`: https://cloudinit.readthedocs.io/en/latest/topics/datasources/nocloud.html
