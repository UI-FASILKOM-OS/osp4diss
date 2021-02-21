	---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](InstallVirtualBox.md)
[NEXT](DebianGuestExportOva.md)

# Creating a Debian Guest on VirtualBox

## NOTE: Version <span style="color:red; font-weight:bold; font-size:larger;">Debian 10.5</span>

## <span style="color:red; font-weight:bold; font-size:larger;">THIS IS SUBJECT TO CHANGE!</span>

<br>
[Part 1: Creating a New Guest](#part-1-creating-a-new-guest)
<br>
[Part 2: Setting the New Guest](#part-2-setting-the-new-guest-in-this-example-osp205)

## Part 1: Creating a New Guest

* You should adjust these following according to your own belief and faith.
  * **OSPD105** = Operating System Programming with Debian 10.5 (<span style="color:red; font-weight:bold; font-size:larger;">your version may be different</span>).
  * Memory = 1024 MB (512MB is OK!)
  * Storage = 8 GB (dynamically allocated)
  * NAT from host (127.0.0.1 port 6022) to guest (10.0.2.15 port 22)

<br>
## Click NEW

<img src="pictures/A-OSP-18.jpg"  width="960">

<br>
* Name = **OSPD105** (Operating System Programming with Debian 10.5)
  * Type: Linux
  * Version: Debian (64bit)

<img src="pictures/A-OSP-19.jpg"  width="960">

<br>
* Memory size = <span style="color:red; font-weight:bold; font-size:larger;">1024 MB</span> (But, 512 MB is OK too!)

<img src="pictures/A-OSP-20.jpg"  width="960">

<br>
* Create a Virtual Hard Disk

<img src="pictures/A-OSP-21.jpg"  width="960">

<br>
* Hard Disk type: VDI

<img src="pictures/A-OSP-22.jpg"  width="960">

<br>
* Storage: Dynamically Allocated

<img src="pictures/A-OSP-23.jpg"  width="960">

<br>
* Storage = 8 GB (dynamically allocated)

<img src="pictures/A-OSP-24.jpg"  width="960">

<br>
## Part 2: Setting the New Guest (In this example OSP205)

### Click SETTING

<img src="pictures/A-OSP-25.jpg"  width="960">

<br>
### General: Basic

<img src="pictures/A-OSP-26.jpg"  width="960">

<br>
### General: Advanced

<img src="pictures/A-OSP-27.jpg"  width="960">

<br>
### System: Motherboard

<img src="pictures/A-OSP-29.jpg"  width="960">

<br>
### System: Processor

### 6 Cores (Depends on how many cores are available)

<img src="pictures/A-OSP-30.jpg"  width="960">

<br>
### System: Acceleration

<img src="pictures/A-OSP-31.jpg"  width="960">

<br>
### Display: Screen

<img src="pictures/A-OSP-32.jpg"  width="960">

<br>
### Storage: Remove Empty IDE
* RIGHT click

<img src="pictures/A-OSP-28a.jpg"  width="960">

* Remove Empty

<img src="pictures/A-OSP-28b.jpg"  width="960">

<br>
### Storage: SATA

<img src="pictures/A-OSP-33.jpg"  width="960">

<br>
### Storage: SATA: Add Debian NetInst ISO image (Eg. <span style="color:red; font-weight:bold; font-size:larger;">debian-10.5.0-amd64-netinst.iso</span>)

<br>
<img src="pictures/A-OSP-34a.jpg"  width="960">
<br>
<img src="pictures/A-OSP-34b.jpg"  width="960">
<br>
<img src="pictures/A-OSP-34c.jpg"  width="960">

<br>
### Network: Adapter 1 (NAT): Port Forwarding

* Click Advanced

<img src="pictures/A-OSP-35.jpg"  width="960">

<br>
### Network: Adapter 1 (NAT)

* **ADD (+)** Forward ssh from host 127.0.0.1:6022 to guest 10.0.2.15:22

<img src="pictures/A-OSP-36.jpg"  width="960">

<img src="pictures/A-OSP-37.jpg"  width="960">

<br>
## OSP105 is DONE!

<img src="pictures/F-OSP-05.jpg"  width="960">

<br>
# The SHORTCUT

<span style="color:red; font-weight:bold; font-size:larger;">
For a limited time only!
If you are rushing, you might want to download this following OVA file.
No purchase necessary and void where prohibited.
Hurry, Google might not like it if too many downloads a huge file. 
</span>

* **README1**:  [https://bit.ly/3mxkpvP](https://bit.ly/3mxkpvP) (182 bytes)

* **Debian 10.5 OVA for VirtualBox**: [https://bit.ly/2FMU7F8](https://bit.ly/2FMU7F8) (662MB)

* **README2**: [https://bit.ly/30ysAP5](https://bit.ly/30ysAP5) (249 bytes)

* **Ubuntu Server 20.04 for VirtualBox**: [https://bit.ly/2HRIihL](https://bit.ly/2HRIihL) (1.2GB)

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](InstallVirtualBox.md)
[NEXT](DebianGuestExportOva.md)
<br>

