<br>
## LFS Chapter 8. Installing Basic System Software

* Split chapter 8 into parts:
  * Chapter 8.01 - 08.17 (LFS-08-01.ova)
  * Chapter 8.18 - 08.25 (LFS-08-18.ova)
  * Chapter 8.26 - 08.30 (LFS-08-26.ova)
  * Chapter 8.31 - 08.40 (LFS-08-31.ova)
  * Chapter 8.41 - 08.60 (LFS-08-41.ova)
  * Chapter 8.61 - 08.78 (LFS-08-61.ova)
* See the scripts at <https://github.com/cbkadal/os211quiz/tree/master/SandBox/W10/>.
  * Always start a part with a "do" script. 
  * Check/learn/modify the script berfore using it!
  * Run the script in a separated terminal.
  * Do not run the script with "lfs" or "root"!
  * See reports examples at <https://github.com/cbkadal/os211quiz/tree/master/SandBox/W10/W10/>.
* User "lfs" and/or "root" to Install the Basic System Software
  * Chroot before starting every part.
  * Follow <https://www.linuxfromscratch.org/lfs/view/10.1/chapter08/chapter08.html>.
  * See also
    * <https://www.youtube.com/watch?v=cmH5B7LjhoE>,
    * <https://lfs.vlsm.org/LFS-08-01.html>,
    * <https://lfs.vlsm.org/LFS-08-18.html>,
    * <https://lfs.vlsm.org/LFS-08-26.html>,
    * <https://lfs.vlsm.org/LFS-08-31.html>,
    * <https://lfs.vlsm.org/LFS-08-41.html>,
    * <https://lfs.vlsm.org/LFS-08-61.html>.
* Always cancel (Control-C) the scipt at the end of the part.
  * Save the result into ~/RESULT/W10/

<br>
## FINALE REPORT
* Before shutdown, run "do_ch8_FINALE.sh"
  * Save the result into ~/RESULT/W10/

<br>
### Update "TXT/myscript.sh"
* Modify "myscript.sh" to automate the tarball encryption process.
* See also <https://cbkadal.github.io/os211/004.html>.
* tar and compress the "W09/" directory into "myW10.tar.bz2"
  * See also [How to create a TARBALL](osp-001.md).
* gnupg asymetric encryption and armor TARBALL "myW10.tar.bz2" for "operatingsystems@vlsm.org" and "yourself".
* the result "myW10.tar.bz2.asc" should be placed into the "TXT/" folder.

```
cd $HOME/git/os211/TXT/
ls -al
bash myscript.sh
ls -al

```



<br>
## Do the "4 git mantra": pull, add, commit, push.

```
git pull; git add -A; git commit -m "OS211 cbkadal"; git push;

```

<br>
## Update your log
* Eg. <https://cbkadal.github.io/os211/TXT/mylog.txt>.

<br>
## CHECK LIST

```
HOMEPAGE: links to W01/, W02/, W03/, W04/, W05/, W06/, W07/, W08/, W09/, W10/.
Top10 Files: w01.md, w02.md, w03.md, w04.md, w05.md, w06.md, w07.md, w08.md, w09.md.
Tip File: w10.md.
TXT/mypubkey.txt: Public Key.
TXT/myrank.txt: Top10 review up to Week09.
WEEK10-REPORT-CH08_01.txt (assignment).
WEEK10-REPORT-CH08_18.txt (assignment).
WEEK10-REPORT-CH08_26.txt (assignment).
WEEK10-REPORT-CH08_31.txt (assignment).
WEEK10-REPORT-CH08_41.txt (assignment).
WEEK10-REPORT-CH08_61.txt (assignment).
WEEK10-REPORT-CH08_FINALE.txt (assignment).
TXT/myscript.sh: A script to automate the process.
TARBALLS: myW03.tar.bz2.asc, myW04.tar.bz2.asc, myW05.tar.bz2.asc, 
myW06.tar.bz2.asc, myW07.tar.bz2.asc, myW08.tar.bz2.asc, 
myW09.tar.bz2.asc, myW10.tar.bz2.asc (assignments).
TXT/mylog.txt: Log Update.
Checksum: SHA256SUM .
Signature: SHA256SUM.asc.

```

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](W08.md)
[NEXT](osp-001.md)
<br>

