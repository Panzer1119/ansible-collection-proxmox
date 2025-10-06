# Panzer1119 Proxmox Collection Release Notes

<a id="v0-4-1"></a>
## v0\.4\.1

<a id="bugfixes"></a>
### Bugfixes

* pbs\_web\_interface\_qol\_patch \- Allow version check command to run in check mode\.
* pve\_web\_interface\_qol\_patch \- Allow version check command to run in check mode\. Fix version extraction\.

<a id="v0-4-0"></a>
## v0\.4\.0

<a id="major-changes"></a>
### Major Changes

* pbs\_web\_interface\_qol\_patch \- Check for Proxmox Backup Server version 3 and adjust patching accordingly\.
* pve\_web\_interface\_qol\_patch \- Check for Proxmox VE version 8 and adjust patching accordingly\.

<a id="v0-3-3"></a>
## v0\.3\.3

<a id="bugfixes-1"></a>
### Bugfixes

* pve\_set\_up\_ansible\_user \- Switch to mapping the list of allowed lxc ids to commands instead of looping over it\. Because the loop executes the task multiple times\, it would overwrite the sudoers file multiple times\, resulting in only the last entry being present\.

<a id="v0-3-2"></a>
## v0\.3\.2

<a id="bugfixes-2"></a>
### Bugfixes

* pve\_set\_up\_ansible\_user \- Fixed an indentation error in the sudoers configuration task that prevented the looping\.

<a id="v0-3-1"></a>
## v0\.3\.1

<a id="bugfixes-3"></a>
### Bugfixes

* pve\_set\_up\_ansible\_user \- Fixed an issue where the variable <code>ansible\_user</code> was used\, despite it being a reserved Ansible variable\. This has been replaced with <code>proxmox\_user</code> to avoid conflicts\.

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
