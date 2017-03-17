# PSUpgradeWindows10
Powershell module for remote in-place upgrades of Windows 7/8 to Windows 10.

# Overview
This module will use a combination of tools including Powershell, PSExec, and Microsoft Deployment Toolkit in order to remotely in-place upgrades domain-joined Windows machines to Windows 10. The main use case for this module is a work around for the requirement of in-place upgrades with MDT that require interactive logons and to launch the litetouch.vbs script. To get around this requirement we use PowerShell workflow and PSMSTSC to launch a Remote Desktop session to each computer, then launch litetouch.vbs with PSExec. This is admittedly a complete hack and I offer no guarantee to any user of this module. With that said, I plan on using this.


