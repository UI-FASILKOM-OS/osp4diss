---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](UpdateDebian.md)
[NEXT](Welcome2GNULinux.md)

# More Debian Packages

## SSH into the GUEST

* UserName: cbkadal (or whatever)

```
ssh -p 6022 cbkadal@localhost
```

<img src="pictures/H-OSP-08.jpg"  width="960">

```
# You need the "root" password
su -
# Update/Upgrade
apt-get update; apt-get dist-upgrade -y;
```
<br>
## The Package List

```
export DEBS="
aptitude
autoconf
automake 
bc
bison
build-essential
curl
fakeroot
flex
fuse 
git
gnupg
libacl1-dev
libcap-dev
libelf-dev
libfuse-dev
libncurses-dev
libseccomp-dev
libselinux1-dev
libssl-dev
lynx
make
manpages
manpages-dev
net-tools
nvi
p7zip-full
pkg-config
rsync
sshfs
sysstat
vim
wget
"

```
<br>
## Install the package list above

```
apt-get install $DEBS -y
```

<img src="pictures/H-OSP-12.jpg"  width="960">

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](UpdateDebian.md)
[NEXT](Welcome2GNULinux.md)
<br>

