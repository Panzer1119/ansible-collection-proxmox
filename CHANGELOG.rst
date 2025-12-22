===========================================
Panzer1119 Proxmox Collection Release Notes
===========================================

.. contents:: Topics

v0.7.0
======

Major Changes
-------------

- pve_web_interface_qol_patch - Add support for Proxmox Virtual Environment 9.0

v0.6.1
======

Minor Changes
-------------

- pbs_web_interface_qol_patch - Add option to skip version check.
- pve_web_interface_qol_patch - Add option to skip version check.

v0.6.0
======

Major Changes
-------------

- pbs_web_interface_qol_patch - Add support for Proxmox Backup Server 4.0

v0.5.2
======

Bugfixes
--------

- pbs_web_interface_qol_patch - Fix tasks.

v0.5.1
======

Bugfixes
--------

- pbs_web_interface_qol_patch - Add support for Proxmox Backup Server 3.4.

v0.5.0
======

Minor Changes
-------------

- pbs_web_interface_qol_patch - Add support for Proxmox Backup Server 3.4.
- pve_web_interface_qol_patch - Add support for Proxmox VE 8.4.

Bugfixes
--------

- pve_web_interface_qol_patch - Fix version extraction.

v0.4.2
======

Bugfixes
--------

- pbs_web_interface_qol_patch - Correct typo.

v0.4.1
======

Bugfixes
--------

- pbs_web_interface_qol_patch - Allow version check command to run in check mode.
- pve_web_interface_qol_patch - Allow version check command to run in check mode. Fix version extraction.

v0.4.0
======

Major Changes
-------------

- pbs_web_interface_qol_patch - Check for Proxmox Backup Server version 3 and adjust patching accordingly.
- pve_web_interface_qol_patch - Check for Proxmox VE version 8 and adjust patching accordingly.

v0.3.3
======

Bugfixes
--------

- pve_set_up_ansible_user - Switch to mapping the list of allowed lxc ids to commands instead of looping over it. Because the loop executes the task multiple times, it would overwrite the sudoers file multiple times, resulting in only the last entry being present.

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
