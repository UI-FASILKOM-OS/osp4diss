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

# PUTTY, WINSCP and SSH

<br>
## FDM: Free Download Manager (Optional)

<span style="color:red; font-weight:bold; font-size:larger;">
Use Free Download Manager if your internet link is slow and less reliable.
Otherwise, download with a regular browser like Firefox or you can install the <b>plugin</b> for that browser.
</span>

### See also [FDM: Free Download Manager (Optional)](http://localhost:4000/InstallFDM.html)

<br>
## Downloading PUTTY

### PUTTY URL: [https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

* In this example, the version is <span style="color:red; font-weight:bold; font-size:larger;">PUTTY 0.74</span>

<img src="pictures/WK-OSP-00.jpg"  width="960">

* Free Download Manager

<img src="pictures/WK-OSP-01.jpg"  width="960">

<br>
## Downloading WINSCP

### WinSCP URL: [https://winscp.net/eng/download.php](https://winscp.net/eng/download.php)

* In this example, the version is <span style="color:red; font-weight:bold; font-size:larger;">WinSCP 5.17</span>

<img src="pictures/WK-OSP-02.jpg"  width="960">

* Free Download Manager

<img src="pictures/WK-OSP-03.jpg"  width="960">

* ZZZ... waiting...

<img src="pictures/WK-OSP-04.jpg"  width="960">

* Done

<img src="pictures/WK-OSP-05.jpg"  width="960">

<br>
<br>
<hr>
<span style="color:red; font-weight:bold; font-size:larger;">
Make sure to start your Debian Guest before trying to connect (putty/ssh) to it.
</span>
<hr>
<br>
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

