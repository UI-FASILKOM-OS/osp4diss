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
## Set a tunnel from osp (port 6023) to badak (ssh port 22) via kawung (ssh port XYZZY).

```
ssh -p XYZZY -L 6023:badak.cs.ui.ac.id:22 cbkadal@kawung.cs.ui.ac.id

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
## Cloning a github repository "os221"

<img src="pictures/cbkadal-06.jpg" width="960">

<br>
```
cd
gitstat
mkdir git
cd git
git clone https://github.com/cbkadal/os221.git
gitstat
cd git
gitstat

```

<img src="pictures/cbkadal-08.jpg" width="960">

<br>
## Cloning a github repository "SistemOperasi"

<img src="pictures/cbkadal-09.jpg" width="960">

<br>
### INPUT01
```
cd 
cd git
gitstat
git clone https://github.com/UI-FASILKOM-OS/SistemOperasi.git
gitstat
cd SistemOperasi
gitstat

```

<br>
### OUTPUT01
```
cbkadal@osp:~$ cd 

cbkadal@osp:~$ cd git

cbkadal@osp:~/git$ gitstat
./  ../  os211/  .shsh  xchg211/  .ZREMOTE/
ZCZC cbkadal ==== Sun 28 Feb 17:06:16 WIB 2021 ===== PWD:/home/cbkadal/git

cbkadal@osp:~/git$ git clone https://github.com/UI-FASILKOM-OS/SistemOperasi.git
Cloning into 'SistemOperasi'...
remote: Enumerating objects: 119, done.
remote: Counting objects: 100% (119/119), done.
remote: Compressing objects: 100% (69/69), done.
remote: Total 5774 (delta 67), reused 76 (delta 50), pack-reused 5655
Receiving objects: 100% (5774/5774), 105.23 MiB | 2.14 MiB/s, done.
Resolving deltas: 100% (4296/4296), done.

cbkadal@osp:~/git$ gitstat
./  ../  os211/  .shsh  SistemOperasi/  xchg211/  .ZREMOTE/
ZCZC cbkadal ==== Sun 28 Feb 17:07:11 WIB 2021 ===== PWD:/home/cbkadal/git

cbkadal@osp:~/git$ cd SistemOperasi

cbkadal@osp:~/git/SistemOperasi$ gitstat
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
./     _config.yml  .dojekyll    Gemfile     index.md  pib.jpg       SECURITY.md
../    covid.md     faq.md       .git/       LICENSE   playlists.md  Slides/
CNAME  Demos/       favicon.ico  .gitignore  Log/      README.md@    WEEK/
ZCZC cbkadal ==== Sun 28 Feb 17:08:11 WIB 2021 ===== PWD:/home/cbkadal/git/SistemOperasi
cbkadal@osp:~/git/SistemOperasi$ 

```

<br>
### INPUT02
```
cd
pwd
mkdir mydemo
cp -r git/SistemOperasi/Demos/Week01/ mydemo/
ls -F mydemo/Week01/

```

<br>
### OUTPUT02
```
cbkadal@osp:~/git/SistemOperasi$ cd

cbkadal@osp:~$ pwd
/home/cbkadal

cbkadal@osp:~$ mkdir mydemo

cbkadal@osp:~$ cp -r git/SistemOperasi/Demos/Week01/ mydemo/

cbkadal@osp:~$ ls -F mydemo/Week01/
000-READ-THIS-FIRST.txt  a05-finding-EXIST  a10-mysha1   a15-uts171  a20-uts201
a01-SCREEN-CHECK         a06-loop           a11-banding  a16-uts181
a02-sort-n-prepare       a07-tester         a12-fixfs    a17-uts182
a03-command-lines-demo   a08-append-a-file  a13-last     a18-uts191
a04-does-it-exist        a09-add-numbers    a14-absen    a19-uts192
cbkadal@osp:~$ 

```

<br>
## Updating mylog.txt

```
cd
gitstat
cd git/os211/TXT
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
git commit -m "OS211 cbkadal UPDATE mylog.txt"
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

