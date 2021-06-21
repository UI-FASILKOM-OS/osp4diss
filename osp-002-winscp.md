---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](ExportImportGuests.md)
[NEXT](UpdateDebian.md)

# Starting a Debian Guest (Eg. D105-W200831)

<img src="pictures/WK-OSP-06.jpg"  width="960">

<img src="pictures/H-OSP-04.jpg"  width="960">

<img src="pictures/H-OSP-05.jpg"  width="960">

<br>
## HIT "ALT-F1"

* login from console (tty1) as "root"

<img src="pictures/WK-OSP-07.jpg"  width="960">

<br>
* who is there (w)

```
w

```
<br>

<img src="pictures/WK-OSP-08.jpg"  width="960">

<br>
## HIT "ALT-F2"

* login from tty2 as "cbkadal" (or whatever your username is)
* who is there (w)

```
w

```

<br>
<img src="pictures/WK-OSP-09.jpg"  width="960">

<br>
## PUTTY

<img src="pictures/WK-OSP-10.jpg"  width="960">

<br>
* localhost:6022
* save as "OSP"

<img src="pictures/WK-OSP-11.jpg"  width="960">

<br>
* change Appearance

<img src="pictures/WK-OSP-12.jpg"  width="960">

<br>
* Courier New, Bold, 18pt (or else)

<img src="pictures/WK-OSP-13.jpg"  width="960">

<br>
* Save and Open

<img src="pictures/WK-OSP-14.jpg"  width="960">

<br>
* Security Alert (First Time)

<img src="pictures/WK-OSP-15.jpg"  width="960">

<br>
* login as cbkadal
* who is there (w)

```
w

```
<br>

<img src="pictures/WK-OSP-16.jpg"  width="960">
<br>

```
exit

```
<br>

<img src="pictures/WK-OSP-17.jpg"  width="960">

<br>
## ALT-F1 (console/tty1)

* shutdown from console/tty1

```
shutdown -h now

```

<img src="pictures/WK-OSP-18.jpg"  width="960">

<br>
## OR: ACPI SHUTDOWN

<img src="pictures/WK-OSP-19.jpg"  width="960">

<hr>


<br>
## SSH from a GNU/Linux HOST

```
ssh -p 6022 osp@localhost
# REMOVE THE OLD KEY
ssh-keygen -f ~/.ssh/known_hosts -R "[localhost]:6022"

```

<img src="pictures/H-OSP-07.jpg"  width="960">

```
# ONE MORE TIME
ssh -p 6022 cbkadal@localhost

```

<img src="pictures/H-OSP-08.jpg"  width="960">

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](ExportImportGuests.md)
[NEXT](UpdateDebian.md)
<br>

