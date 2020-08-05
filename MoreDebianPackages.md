---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)

# More Debian Packages

## SSH into the GUEST

```
ssh -p 6022 osp@localhost
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
fakeroot
flex
fuse 
git
gnupg
libelf-dev
libfuse-dev
libncurses-dev
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

<img src="pictures/H-OSP-11.jpg"  width="960">

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
<br>

