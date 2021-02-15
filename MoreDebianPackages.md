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
apt-file
apt-transport-https
aptitude
autoconf
automake 
bc
bison
bridge-utils
build-essential
ca-certificates
cgroupfs-mount
coreutils
curl
dns-root-data
dnsmasq-base
docker.io
fakeroot
flex
fuse 
gawk
git
git-flow
gnupg
gnupg-agent
libacl1-dev
libcap-dev
libelf-dev
libfuse-dev
libncurses-dev
libseccomp-dev
libselinux1-dev
libssl-dev
locales-all
lynx
make
manpages
manpages-dev
module-assistant
net-tools
nvi
p7zip-full
parted
pigz
pkg-config
runc
ssh
software-properties-common
rsync
sshfs
sysstat
texinfo
vim
wget
x11-apps
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

