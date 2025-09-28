# Panzer1119 Proxmox Collection Release Notes

**Topics**

- <a href="#v0-3-0">v0\.3\.0</a>
    - <a href="#release-summary">Release Summary</a>
    - <a href="#new-roles">New Roles</a>
- <a href="#v0-2-0">v0\.2\.0</a>
    - <a href="#release-summary-1">Release Summary</a>
    - <a href="#new-roles-1">New Roles</a>
- <a href="#v0-1-0">v0\.1\.0</a>
    - <a href="#release-summary-2">Release Summary</a>
    - <a href="#new-roles-2">New Roles</a>

<a id="v0-3-0"></a>
## v0\.3\.0

<a id="release-summary"></a>
### Release Summary

Created a role to set up an Ansible user on Proxmox VE hosts\.

<a id="new-roles"></a>
### New Roles

* panzer1119\.proxmox\.pve\_set\_up\_ansible\_user \- Sets up a dedicated Ansible user on Proxmox VE hosts with sudo privileges for pct and SSH key authentication\.

<a id="v0-2-0"></a>
## v0\.2\.0

<a id="release-summary-1"></a>
### Release Summary

Migrated the role pbs\_web\_interface\_qol\_patch from its own repository to this collection\.

<a id="new-roles-1"></a>
### New Roles

* panzer1119\.proxmox\.pbs\_web\_interface\_qol\_patch \- Applies some quality of life improvement patches to the web interface of Proxmox Backup Server

<a id="v0-1-0"></a>
## v0\.1\.0

<a id="release-summary-2"></a>
### Release Summary

Migrated the role pve\_web\_interface\_qol\_patch from its own repository to this collection\.

<a id="new-roles-2"></a>
### New Roles

* panzer1119\.proxmox\.pve\_web\_interface\_qol\_patch \- Applies some quality of life improvement patches to the web interface of Proxmox VE
