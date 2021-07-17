---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/OSP4DISS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)

<br id="idx00"><br>
Welcome to the Operating System Programming for DISS site.
The following is a step-by-step guide to set up a Virtual Debian Guest on VirtualBox.

<br id="idx00a">
# TOC

* [Introduction](#idx00)
* [VirtualBox Guest Preparation](#idx00a)
* [Import/Export/Delete a Virtual Guest](#idx01)
* [Importing OVA or Installing ISO?](#idx02)
  * [Option 1: Importing a VirtualBox Debian Guest (OVA File)](#idx02a)
  * [Option 2: Installing a VirtualBox Debian Guest (ISO File)](#idx02b)
* [Running a VirtualBox Debian Guest (both OVA or ISO](#idx03)
* [Dress Up Your Virtual Guest](#idx04)
* [PULL from / PUSH to GitHub](#idx05)

<br id="idx00b">
# VirtualBox Guest Preparation

You need a hypervisor, i.e., VirtualBox.
It can be installed on Windows 10, macOS, or Linux.
Using a Download Manager might help for a less reliable internet connection.
For Windows 10, you also need to install PUTTY and WINSCP.

* [FDM: Free Download Manager (Optional)](InstallFDM.md)
* [Downloading and Installing VirtualBox](InstallVirtualBox.md)
* [Downloading and Installing PUTTY and WINSCP](SSHGuest.md)

<br id="idx01">
# Import/Export/Delete a Virtual Guest

* [Exporting a VirtualBox Guest (OVA)](DebianGuestExportOva.md)
* [Importing a VirtualBox Guest with a different Name](DebianGuestImportOva.md)
* [Export Import VirtualBox Guest(s)](ExportImportGuests.md)
* [Deleting Debian VirtualBox Guest(s)](DebianGuestDeleteOva.md)

<br id="idx02">
# Importing OVA or Installing ISO?

<br id="idx02a">
## Option 1: Importing a VirtualBox Debian Guest (OVA File)

* For importing a Debian 10 OVA Image:
  * [DEBIAN-10.10-README.txt](https://bit.ly/3B12SU6)
  * [DEBIAN-10.10.ova](https://bit.ly/36z3diC) (346 MB)

<br id="idx02b">
## Option 2: Installing a VirtualBox Debian Guest (ISO File)

* [VirtualBox: NEW EMPTY Guest with 2 x 64GB disks](DebianGuestOnVirtualBox1.md) (E.g. DEB10-00-0-64G+64G-EMPTY)
* [VirtualBox: General](DebianGuestOnVirtualBox2.md)
* [VirtualBox: System](DebianGuestOnVirtualBox3.md)
* [VirtualBox: Display](DebianGuestOnVirtualBox4.md)
* [VirtualBox: Storage](DebianGuestOnVirtualBox5.md)
* [VirtualBox: Audio](DebianGuestOnVirtualBox6.md)
* [VirtualBox: Network](DebianGuestOnVirtualBox7.md)
* [Downloading Debian ISO Image](DebianISOImage.md)
* [Installing Debian Netinst Guest on VirtualBox](InstallDebianNetinst.md)
* Export your Virtual Guest as "DEB00-00-1-INSTALL.ova"

<br id="idx03">
# Running a VirtualBox Debian Guest (both OVA or ISO)

* Import "DEBIAN-10.10.ova" (Option 1) or "DEB00-00-1-INSTALL.ova" (Option 2).
* Rename your Virtual Guest as "Guest-01a".
* [Startup a VirtualBox Guest](osp-002-startup.md)
* [Shutdown a VirtualBox Guest](osp-002-shutdown.md)
* [Login from a Console](osp-002-login.md)
* [Login with PUTTY](osp-002-putty.md)
* [Login with SSH](osp-002-ssh.md)
* [WINSCP](osp-002-winscp.md)
* [SCP](osp-002-scp.md)
* **Tutorial**:
  [Study some Command Lines, Editor, Regular Expression (regex), and String Processing](Welcome2GNULinux.md)
* Export your virtual guest to an OVA file. E.g. "Guest-01a.ova".

<br id="idx04">
# Dress Up Your Virtual Guest

* Import your virtual guest from "Guest-01a.ova".
* Rename the Guest to "Guest-01b".
* [Update Your Debian Guest](osp-102.md)
* [Adding Debian Packages](osp-103.md)
* [Adding UserName](osp-104.md) -- E.g. "dummy" and "CicakBinKadal"
* [Rename Hostname](osp-105.md)
* [.bash_profile](osp-106.md)
* [.vimrc](osp-107.md)
* [.bash_aliases](osp-108.md)
* [SUPERUSER](osp-109.md)
* Export your virtual guest to an OVA file. E.g. "Guest-01b.ova".

<br id="idx05">
# PULL from / PUSH to GitHub.com

* Import your virtual guest from "Guest-01b.ova".
* Rename the Guest to "Guest-01c".
* [SSH: Generating public/private rsa key pair](osp-110.md)
* [SSH: Put a Public Key at GitHub.com](osp-111.md)
* Export your virtual guest to an OVA file. E.g. "Guest-01c.ova".

<br>
# Assignments

* [Cicak Bin Kadal part 01](CBKadal.md)
* [Cicak Bin Kadal part 02](CBKadal2.md)
* [Cicak Bin Kadal Assignment Week 03](W03.md)
* [Cicak Bin Kadal Assignment Week 04](W04.md)
* [Cicak Bin Kadal Assignment Week 05](W05.md)
* [Cicak Bin Kadal Assignment Week 06](W06.md)
* [Cicak Bin Kadal Assignment Week 07](W07.md)
* [Cicak Bin Kadal Assignment Week 08](W08.md)
* [Cicak Bin Kadal Assignment Week 09](W09.md)
* [Cicak Bin Kadal Assignment Week 10](W10.md)

<br>
# PLUGH
* [Making and encrypting a tarball](osp-001.md)
* [FUSE Demo](osp-100.md)
* [TOP Demo](osp-101.md)
* [Windows10 (Kleopatra)](CBKadal3.md)
* [Log Codes](ETC/logCodes.txt)
* [OS Public Key](ETC/ospubkey.txt)
* [X11 Windows 10](osp-003.md)

<br>
<hr>
<br id="endofpage"><br>

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/OSP4DISS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
<br>


