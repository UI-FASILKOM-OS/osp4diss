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

## NOTE: Version <span style="color:red; font-weight:bold; font-size:larger;">Debian 10.7</span>

## <span style="color:red; font-weight:bold; font-size:larger;">THIS IS SUBJECT TO CHANGE!</span>

<br>
[Part 1: Creating a New Guest](#part-1-creating-a-new-guest)
<br>
[Part 2: Setting the New Guest](#part-2-setting-the-new-guest-in-this-example-deb10-00-0-64g64g-empty)
<br>
[Part 3: Export OVA](#part-3-export-ova)
<br>
[Part 4: Import (Rename) OVA](#part-4-import-rename-ova)
<br>
[Part 5: The Short Cut](#part-5-the-short-cut)

## Part 1: Creating a New Guest

* You should adjust these following according to your own belief and faith.
  * Name: **DEB10-00-0-64G+64G-EMPTY** (<span style="color:red; font-weight:bold; font-size:larger;">your version may be different</span>).
  * Memory = 1024 MB (512MB is OK too!)
  * Storage1 = 64 GB (dynamically allocated)
  * Storage2 = 64 GB (dynamically allocated)
  * SSH: NAT  from host  (127.0.0.1 port 6022) to guest (10.0.2.15 port 22)
  * Jekyll: NAT from host (127.0.0.1 port 5000) to guest (10.0.2.15 port 4000)

<br>
## Click NEW

<img src="pictures/osp21-00.jpg"  width="960">

<br>
* Name = **DEB10-00-0-64G+64G-EMPTY**
  * Type: Linux
  * Version: Debian (64bit)

<img src="pictures/osp21-01.jpg"  width="960">

<br>
* Memory size = <span style="color:red; font-weight:bold; font-size:larger;">1024 MB</span> (But, 512 MB is OK too!)

<img src="pictures/osp21-02.jpg"  width="960">

<br>
* Create a Virtual Hard Disk

<img src="pictures/osp21-03.jpg"  width="960">

<br>
* Hard Disk type: VDI

<img src="pictures/osp21-04.jpg"  width="960">

<br>
* Storage: Dynamically Allocated

<img src="pictures/osp21-05.jpg"  width="960">

<br>
* Storage = 64 GB (dynamically allocated)

<img src="pictures/osp21-06.jpg"  width="960">

<br>
## Part 2: Setting the New Guest (In this example **DEB10-00-0-64G+64G-EMPTY**)

### Click SETTING

<img src="pictures/osp21-07.jpg"  width="960">

<br>
### General: Basic

<img src="pictures/osp21-08.jpg"  width="960">

<br>
### General: Advanced

<img src="pictures/osp21-09.jpg"  width="960">

<br>
### System: Motherboard

<img src="pictures/osp21-10.jpg"  width="960">

<br>
### System: Processors (6)

<img src="pictures/osp21-11.jpg"  width="960">

<br>
### System: Acceleration

<img src="pictures/osp21-12.jpg"  width="960">

<br>
### Display: Screen

* Scale Factor: 150%

<img src="pictures/osp21-13.jpg"  width="960">

<br>
### Storage: Remove Empty IDE

* RIGHT click (Remove Attachment)

<img src="pictures/osp21-14.jpg"  width="960">

* Remove Empty 

<img src="pictures/osp21-15.jpg"  width="960">

<br>
### Storage: SATA: Adds Hard disk

<img src="pictures/osp21-16.jpg"  width="960">

* Create a new disk

<img src="pictures/osp21-17.jpg"  width="960">

* Hard disk type: VDI

<img src="pictures/osp21-18.jpg"  width="960">

* Dynamically Allocated

<img src="pictures/osp21-19.jpg"  width="960">

* (Second) Disk Storage: 64 GB

<img src="pictures/osp21-20.jpg"  width="960">

* Choose (64 GB Storage)

<img src="pictures/osp21-21.jpg"  width="960">

* Sellect IDE Controller

<img src="pictures/osp21-22.jpg"  width="960">

* Remove IDE Controller

<img src="pictures/osp21-23.jpg"  width="960">

<br>
### Audio

<img src="pictures/osp21-24.jpg"  width="960">

* (Nothing)

<img src="pictures/osp21-25.jpg"  width="960">

<br>
### Network: Adapter 1 (NAT): Port Forwarding

* Click Port Forwarding

<img src="pictures/osp21-26.jpg"  width="960">

* **ADD (+)** Forward ssh from host 127.0.0.1:6022 to guest 10.0.2.15:22 (SSH)

<img src="pictures/osp21-27.jpg"  width="960">

* **ADD (+)** Forward ssh from host 127.0.0.1:5000 to guest 10.0.2.15:4000 (Jekyll)

<img src="pictures/doit-008.jpg"  width="960">

<br>
### Network: Adapter 1 (NAT) --- DONE

<img src="pictures/osp21-28.jpg"  width="960">

<br>
## DEB10-00-0-64G+64G-EMPTY is DONE!

<img src="pictures/osp21-30.jpg"  width="960">

## Part 3: Export OVA

<img src="pictures/osp21-31.jpg"  width="960">

* Export Your Guest

<img src="pictures/osp21-32.jpg"  width="960">

* Next

<img src="pictures/osp21-33.jpg"  width="960">

* Export

<img src="pictures/osp21-34.jpg"  width="960">

* Done

<img src="pictures/osp21-35.jpg"  width="960">

## Part 4: Import (Rename) OVA

<img src="pictures/osp21-36.jpg"  width="960">

* Select an OVA file

<img src="pictures/osp21-37.jpg"  width="960">

<img src="pictures/osp21-38.jpg"  width="960">

* DEB10-00-1-INSTALL

<img src="pictures/osp21-39.jpg"  width="960">

* DEB10-00-1-INSTALL

<img src="pictures/osp21-40.jpg"  width="960">

[](ZCZC)


<br>
## Part 5: The Short Cut

<span style="color:red; font-weight:bold; font-size:larger;">
For a limited time only!
If you are rushing, you might want to download this following OVA file.
No purchase necessary and void where prohibited.
Hurry, Google might not like it if too many downloads a huge file. 
</span>

* **README**:  <https://bit.ly/3dszYmt> (371 bytes)

* **Debian 10.7 OVA for VirtualBox**: <https://bit.ly/3saZpgr> (1.1 GB)

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

