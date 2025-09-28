===========================================
Panzer1119 Proxmox Collection Release Notes
===========================================

.. contents:: Topics

v0.3.2
======

Bugfixes
--------

- pve_set_up_ansible_user - Fixed an indentation error in the sudoers configuration task that prevented the looping.

v0.3.1
======

Bugfixes
--------

- pve_set_up_ansible_user - Fixed an issue where the variable ``ansible_user`` was used, despite it being a reserved Ansible variable. This has been replaced with ``proxmox_user`` to avoid conflicts.

v0.3.0
======

Release Summary
---------------

Created a role to set up an Ansible user on Proxmox VE hosts.

New Roles
---------

- panzer1119.proxmox.pve_set_up_ansible_user - Sets up a dedicated Ansible user on Proxmox VE hosts with sudo privileges for pct and SSH key authentication.

v0.2.0
======

Release Summary
---------------

Migrated the role pbs_web_interface_qol_patch from its own repository to this collection.

New Roles
---------

- panzer1119.proxmox.pbs_web_interface_qol_patch - Applies some quality of life improvement patches to the web interface of Proxmox Backup Server

v0.1.0
======

Release Summary
---------------

Migrated the role pve_web_interface_qol_patch from its own repository to this collection.

New Roles
---------

- panzer1119.proxmox.pve_web_interface_qol_patch - Applies some quality of life improvement patches to the web interface of Proxmox VE
