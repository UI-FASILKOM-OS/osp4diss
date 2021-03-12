---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](osp-001.md)
[NEXT](W06.md)

```
<br>
## Create and enter directory "W03/"
```
cbkadal@osp:~$ mkdir W03/

cbkadal@osp:~$ cd W03/

cbkadal@osp:~/W03$ gitstat
./  ../
ZCZC cbkadal ==== Mon 05 Oct 2020 07:49:39 PM WIB ===== PWD:/home/cbkadal/W03

cbkadal@osp:~/W03$ 
```
<br>
## Fetch the TLPI tarball using "wget"

* URL: <https://man7.org/tlpi/code/download/tlpi-200701-dist.tar.gz>

```
cbkadal@osp:~/W03$ wget https://man7.org/tlpi/code/download/tlpi-200701-dist.tar.gz
--2020-10-05 19:49:46--  https://man7.org/tlpi/code/download/tlpi-200701-dist.tar.gz
Resolving man7.org (man7.org)... 45.84.72.15
Connecting to man7.org (man7.org)|45.84.72.15|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 307091 (300K) [application/x-gzip]
Saving to: ‘tlpi-200701-dist.tar.gz’

tlpi-200701-dist.tar.gz       100%[=================================================>] 299.89K   387KB/s    in 0.8s    

2020-10-05 19:49:48 (387 KB/s) - ‘tlpi-200701-dist.tar.gz’ saved [307091/307091]
```
<br>
## List the tarball with "tar".
```
cbkadal@osp:~/W03$ tar tf tlpi-200701-dist.tar.gz 
tlpi-dist/
tlpi-dist/Makefile.inc
tlpi-dist/Makefile

==== TL;DR ====

tlpi-dist/acl/
tlpi-dist/acl/Makefile
tlpi-dist/acl/acl_view.c
tlpi-dist/acl/acl_update.c

cbkadal@osp:~/W03$ gitstat
./  ../  tlpi-200701-dist.tar.gz
ZCZC cbkadal ==== Mon 05 Oct 2020 07:54:24 PM WIB ===== PWD:/home/cbkadal/W03
```
<br>
## Extract the tarball with "tar".
```
cbkadal@osp:~/W03$ tar xf tlpi-200701-dist.tar.gz 

cbkadal@osp:~/W03$ gitstat
./  ../  tlpi-200701-dist.tar.gz  tlpi-dist/
ZCZC cbkadal ==== Mon 05 Oct 2020 07:58:16 PM WIB ===== PWD:/home/cbkadal/W03
```
<br>
## Go to "tlpi-dist/" directory and record the disk usage (du)
```
cbkadal@osp:~/W03$ cd tlpi-dist/

cbkadal@osp:~/W03/tlpi-dist$ du -s -h .
2.6M	.

cbkadal@osp:~/W03/tlpi-dist$ 
```
<br>
## Do "make" and record the disk usage (du)
```
cbkadal@osp:~/W03/tlpi-dist$ make
lib acl altio cap daemons dirs_links filebuff fileio filelock files filesys getopt inotify loginacct memalloc mmap pgsjc pipes pmsg proc proccred procexec procpri procres progconc psem pshm pty shlibs signals sockets svipc svmsg svsem svshm sysinfo syslim threads time timers tty users_groups vdso vmem xattr
make[1]: Entering directory '/home/cbkadal/W03/tlpi-dist/lib'
cc -std=c99 -D_XOPEN_SOURCE=600 -D_DEFAULT_SOURCE -g -I../lib -pedantic -Wall -W -Wmissing-prototypes -Wno-sign-compare -Wimplicit-fallthrough -Wno-unused-parameter   -c -o print_rlimit.o print_rlimit.c

========= TL;DR =========
==== more 400 lines  ====

cc -std=c99 -D_XOPEN_SOURCE=600 -D_DEFAULT_SOURCE -g -I../lib -pedantic -Wall -W -Wmissing-prototypes -Wno-sign-compare -Wimplicit-fallthrough -Wno-unused-parameter    t_setxattr.c ../libtlpi.a   -o t_setxattr
cc -std=c99 -D_XOPEN_SOURCE=600 -D_DEFAULT_SOURCE -g -I../lib -pedantic -Wall -W -Wmissing-prototypes -Wno-sign-compare -Wimplicit-fallthrough -Wno-unused-parameter    xattr_view.c ../libtlpi.a   -o xattr_view
make[1]: Leaving directory '/home/cbkadal/W03/tlpi-dist/xattr'

cbkadal@osp:~/W03/tlpi-dist$ du -s -h .
13M	.
```
<br>
## Do "make clean" and record the disk usage (du)

```
cbkadal@osp:~/W03/tlpi-dist$ make clean
make[1]: Entering directory '/home/cbkadal/W03/tlpi-dist/lib'
rm -f *.o ename.c.inc ../libtlpi.a
make[1]: Leaving directory '/home/cbkadal/W03/tlpi-dist/lib'
make[1]: Entering directory '/home/cbkadal/W03/tlpi-dist/acl'

========= TL;DR =========

rm -f memlock madvise_dontneed t_mprotect  *.o
make[1]: Leaving directory '/home/cbkadal/W03/tlpi-dist/vmem'
make[1]: Entering directory '/home/cbkadal/W03/tlpi-dist/xattr'
rm -f  t_setxattr xattr_view *.o
make[1]: Leaving directory '/home/cbkadal/W03/tlpi-dist/xattr'

cbkadal@osp:~/W03/tlpi-dist$ du -s -h .
2.6M	.
```
<br>
## Put the disk usage record into file myW03disk.txt
```
cbkadal@osp:~/W03/tlpi-dist$ cat myW03disk.txt 
DISK 2.6M 13M 2.6M

cbkadal@osp:~/git/os202/TXT$ 
```
<br>
## Move myW03disk.txt into the github os202 repository

* Always run "myscrit.sh" to update SHA256SUM and SHA256.asc

```
cbkadal@osp:~/git/os202/TXT$ bash myscript.sh 
sha256sum my*.txt my*.sh > SHA256SUM
sha256sum -c SHA256SUM
mylog.txt: OK
mypubkey.txt: OK
myrank.txt: OK
myW03disk.txt: OK
myW03token.txt: OK
myscript.sh: OK
gpg -o SHA256SUM.asc -a -sb SHA256SUM
gpg --verify SHA256SUM.asc SHA256SUM
gpg: Signature made Mon 05 Oct 2020 08:29:00 PM WIB
gpg:                using RSA key C13787F94073986F0FE39A4E6BE9DC2074F27BF1
gpg: Good signature from "Cicak Bin Kadal (CBK) <cbk@dummy>" [ultimate]

cbkadal@osp:~/git/os202/TXT$ ls -al
total 40
drwxr-xr-x 2 cbkadal cbkadal 4096 Oct  5 20:29 .
drwxr-xr-x 5 cbkadal cbkadal 4096 Oct  5 16:54 ..
-rw-r--r-- 1 cbkadal cbkadal  630 Sep 28 18:11 mylog.txt
-rw-r--r-- 1 cbkadal cbkadal 3147 Sep 28 23:25 mypubkey.txt
-rw-r--r-- 1 cbkadal cbkadal  119 Sep 28 21:35 myrank.txt
-rw-r--r-- 1 cbkadal cbkadal  449 Oct  5 17:31 myscript.sh
-rw-r--r-- 1 cbkadal cbkadal   19 Oct  5 20:08 myW03disk.txt
-rw-r--r-- 1 cbkadal cbkadal    5 Oct  5 17:18 myW03token.txt
-rw-r--r-- 1 cbkadal cbkadal  471 Oct  5 20:29 SHA256SUM
-rw-r--r-- 1 cbkadal cbkadal  833 Oct  5 20:29 SHA256SUM.asc

cbkadal@osp:~/git/os202/TXT$ 
```
<br>
## Do the 4 git routine (pull, add, commit, push)
```
cbkadal@osp:~/git/os202/TXT$ git pull; git add -A; git commit -m "OS202 cbkadal"; git push;
Already up to date.
[master 86e99e4] OS202 cbkadal
 3 files changed, 18 insertions(+), 16 deletions(-)
 rewrite TXT/SHA256SUM.asc (91%)
 create mode 100644 TXT/myW03disk.txt
Username for 'https://github.com': cbkadal
Password for 'https://cbkadal@github.com': ******
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 6 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 1.29 KiB | 1.29 MiB/s, done.
Total 6 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/cbkadal/os202.git
   34f65d8..86e99e4  master -> master

cbkadal@osp:~/git/os202/TXT$
```
<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](osp-001.md)
[NEXT](W06.md)
<br>

