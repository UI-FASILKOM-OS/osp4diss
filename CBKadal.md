---
---
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](MoreGNULinux.md)
[NEXT](CBKadal2.md)

# Eg. User: cbkadal

These following examples is for user **cbkadal** of guest *osp*.
Replace **cbkadal** with your own user name.

<br>
## Set a tunnel from osp (port 6023) to badak (ssh port 22) via kawung.

```
ssh -L 6023:badak.cs.ui.ac.id:22 cbkadal@kawung.cs.ui.ac.id
```

<img src="pictures/cbkadal-01.jpg" width="960">

<br>
## Connect to badak via a tunnel.

```
ssh -p 6023 cbkadal@localhost
ls -al /extra/
```
<img src="pictures/cbkadal-02.jpg" width="960">

<br>
## Copy from badak:///extra/ to *osp* via tunnel

```
ls -F
mkdir extra
rsync -auv --delete -e 'ssh -p 6023' cbkadal@localhost:/extra/Docs/  extra/Docs/
```

<img src="pictures/cbkadal-03.jpg" width="960">

<br>
```
rsync -auv --delete -e 'ssh -p 6023' cbkadal@localhost:/extra/Slides/  extra/Slides/
```

<img src="pictures/cbkadal-05.jpg" width="960">

<br>
## Setup git

Config name and email for git.
Replace 'Cicak Bin Kadal' with your own name.

```
gitstat
git config --global user.email        'cbkadal@DELETE.vlsm.org'
git config --global user.name         'Cicak Bin Kadal'
git config --global core.editor       'vi'
git config --global credential.helper 'cache --timeout=3600'
git config user.email
git config user.name
git config core.editor
git config credential.helper
git config --list
cat ~/.gitconfig
gitstat
```
<br>
<img src="pictures/cbkadal-07.jpg" width="960">

<br>
## Cloning a github repository "os202"

<img src="pictures/cbkadal-06.jpg" width="960">

<br>
```
cd
gitstat
mkdir git
cd git
git clone https://github.com/cbkadal/os202.git
gitstat
cd git
gitstat
```

<img src="pictures/cbkadal-08.jpg" width="960">

<br>
## Cloning a github repository "SistemOperasi"

<img src="pictures/cbkadal-09.jpg" width="960">

<br>
```
cd 
cd git
gitstat
git clone https://github.com/UI-FASILKOM-OS/SistemOperasi.git
gitstat
cd SistemOperasi
gitstat
```

<img src="pictures/cbkadal-10.jpg" width="960">

<br>
## Updating mylog.txt

```
cd
gitstat
cd git/os202/TXT
gitstat
vi mylog.txt
```

<img src="pictures/cbkadal-11.jpg" width="960">

<br>
## mylog.txt

<img src="pictures/cbkadal-12.jpg" width="960">

```
gitstat
git add -A
gitstat
```

<img src="pictures/cbkadal-13.jpg" width="960">

```
git commit -m "OS202 cbkadal UPDATE mylog.txt"
gitstat
git pull
git push
git stat
```

<img src="pictures/cbkadal-14.jpg" width="960">

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](MoreGNULinux.md)
[NEXT](CBKadal2.md)

