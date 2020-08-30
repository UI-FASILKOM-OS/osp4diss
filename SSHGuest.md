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

# SSH Guest OSPD104b

<img src="pictures/H-OSP-04.jpg"  width="960">

<img src="pictures/H-OSP-05.jpg"  width="960">

<img src="pictures/H-OSP-06.jpg"  width="960">

<br>
## SSH (or putty) from HOST

```
ssh -p 6022 osp@localhost
# REMOVE THE OLD KEY
ssh-keygen -f ~/.ssh/known_hosts -R "[localhost]:6022"
```

<img src="pictures/H-OSP-07.jpg"  width="960">

```
# ONE MORE TIME
ssh -p 6022 osp@localhost
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

