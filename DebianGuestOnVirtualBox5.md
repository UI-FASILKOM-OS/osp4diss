---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](DebianGuestOnVirtualBox4.md)
[NEXT](DebianGuestOnVirtualBox6.md)

# New VirtualBox Guest: Audio

* Example **DEB10-00-0-64G+64G-EMPTY**

### Click SETTING

<img src="pictures/osp21-07.jpg"  width="960">

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

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](DebianGuestOnVirtualBox4.md)
[NEXT](DebianGuestOnVirtualBox6.md)

