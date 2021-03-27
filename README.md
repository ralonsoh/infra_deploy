Infraestructure deployment
==========================
This project allows to deploy a virtualized infraestructure, using virsh. The
ansible script, using the inventory file defined by the user (e.g.
/etc/config_01.yaml), creates the needed XML files to deploy the networks (using
linux brige) and the virtual machines.

In order to define the user and the password, and the management network
("infra_mgt") configuration, this project uses cloud-init NoCloud [1]_ . This
network is mandatory.

In OpenStack deployments:

* "infra_tenant": is the tenant network, for VLAN or tunneled networks. In
  tunneled networks, the local IP will be the one assigned to the
  "infra_tenant" interface in this machine.
* "infra_ext": is the external (provider) network.


Compatibility
-------------
These are the host OS tested:

* Ubuntu 20.04 server and desktop
* Ubuntu 20.10 desktop

These are the guest OS tested:

* Ubuntu 18.04 server cloud image
* Ubuntu 20.04 server cloud image


Requirements
------------
ansible >= 2.6.4


References
==========
.. [1]: https://cloudinit.readthedocs.io/en/latest/topics/datasources/nocloud.html
