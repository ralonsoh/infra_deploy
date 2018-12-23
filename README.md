..
      Licensed under the Apache License, Version 2.0 (the "License"); you may
      not use this file except in compliance with the License. You may obtain
      a copy of the License at

          http://www.apache.org/licenses/LICENSE-2.0

      Unless required by applicable law or agreed to in writing, software
      distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
      WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
      License for the specific language governing permissions and limitations
      under the License.

      Convention for heading levels in Yardstick documentation:

      =======  Heading 0 (reserved for the title in a document)
      -------  Heading 1
      ~~~~~~~  Heading 2
      +++++++  Heading 3
      '''''''  Heading 4

      Avoid deeper levels because they do not render well.

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
