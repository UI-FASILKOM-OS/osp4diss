---
---
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](CBKadal.md)
[NEXT](CBKadal3.md)

# Eg. User: cbkadal (2)

These following examples is for user **cbkadal** at **osp** (Guest).
Replace **cbkadal** with your own user name.

## Generating a KEY PAIR
* RSA and RSA.
* Keysize is 4096 bits.
* key expires in 1 year.
* No passphrase (**You decide!**).

<br>
### INPUT(1)

```
gpg --full-generate-key

```

### OUTPUT(1)

```
cbkadal@osp:~$ gpg --full-generate-key
gpg (GnuPG) 2.2.12; Copyright (C) 2018 Free Software Foundation, Inc.
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

gpg: directory '/home/cbkadal/.gnupg' created
gpg: keybox '/home/cbkadal/.gnupg/pubring.kbx' created
Please select what kind of key you want:
   (1) RSA and RSA (default)
   (2) DSA and Elgamal
   (3) DSA (sign only)
   (4) RSA (sign only)
Your selection? 1
RSA keys may be between 1024 and 4096 bits long.
What keysize do you want? (3072) 4096
Requested keysize is 4096 bits
Please specify how long the key should be valid.
         0 = key does not expire
      <n>  = key expires in n days
      <n>w = key expires in n weeks
      <n>m = key expires in n months
      <n>y = key expires in n years
Key is valid for? (0) 1y
Key expires at Tue 28 Sep 2021 11:16:14 PM WIB
Is this correct? (y/N) y

GnuPG needs to construct a user ID to identify your key.

Real name: Cicak Bin Kadal
Email address: cbk@dummy
Comment: CBK
You selected this USER-ID:
    "Cicak Bin Kadal (CBK) <cbk@dummy>"

Change (N)ame, (C)omment, (E)mail or (O)kay/(Q)uit? o
We need to generate a lot of random bytes. It is a good idea to perform
some other action (type on the keyboard, move the mouse, utilize the
disks) during the prime generation; this gives the random number
generator a better chance to gain enough entropy.
We need to generate a lot of random bytes. It is a good idea to perform
some other action (type on the keyboard, move the mouse, utilize the
disks) during the prime generation; this gives the random number
generator a better chance to gain enough entropy.
gpg: /home/cbkadal/.gnupg/trustdb.gpg: trustdb created
gpg: key 6BE9DC2074F27BF1 marked as ultimately trusted
gpg: directory '/home/cbkadal/.gnupg/openpgp-revocs.d' created
gpg: revocation certificate stored as '/home/cbkadal/.gnupg/openpgp-revocs.d/XXX.rev'
public and secret key created and signed.

pub   rsa4096 2021-02-18 [SC] [expires: 2021-08-17]
      56754A8214D01B20B97BF5EF078CA2C2F3F22F37
uid           [ultimate] Cicak Bin Kadal (CBK) <cbk@dummy>
sub   rsa4096 2021-02-18 [E] [expires: 2021-08-17]

```

<br>
## List the keys

<br>
### INPUT(2)

```
gpg --list-keys

```

### OUTPUT(2)

```
cbkadal@osp:~$ gpg --list-keys
gpg: checking the trustdb
gpg: marginals needed: 3  completes needed: 1  trust model: pgp
gpg: depth: 0  valid:   2  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 2u
gpg: next trustdb check due at 2021-08-17
--------------------------------
pub   rsa4096 2021-02-18 [SC] [expires: 2021-08-17]
      56754A8214D01B20B97BF5EF078CA2C2F3F22F37
uid           [ultimate] Cicak Bin Kadal (CBK) <cbk@dummy>
sub   rsa4096 2021-02-18 [E] [expires: 2021-08-17]

cbkadal@osp:~$ 

```

<br>
## Importing the Operating Systems public key

* Source: <https://osp4diss.vlsm.org/ETC/ospubkey.txt>

### INPUT(3)

```
wget -c https://osp4diss.vlsm.org/ETC/ospubkey.txt
gpg --import ospubkey.txt
gpg --list-keys

```

### OUTPUT(3)

```
cbkadal@osp:~$ wget -c https://osp4diss.vlsm.org/ETC/ospubkey.txt
--2021-03-08 12:14:19--  https://osp4diss.vlsm.org/ETC/ospubkey.txt
Resolving osp4diss.vlsm.org (osp4diss.vlsm.org)... 185.199.111.153, 185.199.109.153, 185.199.110.153, ...
Connecting to osp4diss.vlsm.org (osp4diss.vlsm.org)|185.199.111.153|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3171 (3.1K) [text/plain]
Saving to: ‘ospubkey.txt’

ospubkey.txt                  100%[=================================================>]   3.10K  --.-KB/s    in 0.001s  

2021-03-08 12:14:20 (5.79 MB/s) - ‘ospubkey.txt’ saved [3171/3171]

cbkadal@osp:~$ gpg --import ospubkey.txt
gpg: key D0F5DBDD67DF6DDE: public key "Operating Systems (OS) <operatingsystems@vlsm.org>" imported
gpg: Total number processed: 1
gpg:               imported: 1

cbkadal@osp:~$ gpg --list-keys
/home/cbkadal/.gnupg/pubring.kbx
--------------------------------
pub   rsa4096 2021-02-18 [SC] [expires: 2021-08-17]
      56754A8214D01B20B97BF5EF078CA2C2F3F22F37
uid           [ultimate] Cicak Bin Kadal (CBK) <cbk@dummy>
sub   rsa4096 2021-02-18 [E] [expires: 2021-08-17]

pub   rsa4096 2020-02-13 [SC] [expires: 2021-08-17]
      B4507B533F7F22840BD8E93ED0F5DBDD67DF6DDE
uid           [ultimate] Operating Systems (OS) <operatingsystems@vlsm.org>
sub   rsa4096 2020-02-13 [E] [expires: 2021-08-17]

```
<br>
## Export Public Key "mypubkey.txt"

<br>
### INPUT(4)

```
cd git/os211/TXT/
rm -f mypubkey.txt
gpg -o mypubkey.txt --armor --export 56754A8214D01B20B97BF5EF078CA2C2F3F22F37
ls -al

```

### OUTPUT(4)

```
cbkadal@osp:~$ cd git/os211/TXT/

cbkadal@osp:~/git/os211/TXT$ rm -f mypubkey.txt

cbkadal@osp:~/git/os211/TXT$ gpg -o mypubkey.txt --armor --export 56754A8214D01B20B97BF5EF078CA2C2F3F22F37

cbkadal@osp:~/git/os211/TXT$ ls -al
total 24
drwxr-xr-x 2 cbkadal cbkadal 4096 Mar  8 12:24 .
drwxr-xr-x 9 cbkadal cbkadal 4096 Mar  7 07:05 ..
-rw-r--r-- 1 cbkadal cbkadal 1171 Mar  8 11:58 mylog.txt
-rw-r--r-- 1 cbkadal cbkadal 3147 Mar  8 12:24 mypubkey.txt
-rw-r--r-- 1 cbkadal cbkadal  491 Mar  5 13:19 myrank.txt
-rw-r--r-- 1 cbkadal cbkadal  453 Mar  5 13:19 myscript.sh

cbkadal@osp:~/git/os211/TXT$ 

```
<br>
## Generate SHA256SUM and SHA256SUM.asc

<br>
### INPUT(5)

```
ls -al
bash myscript.sh 
git pull
git add -A
git commit -m "OS211 cbkadal TXT"
git push
ls -al

```

### OUTPUT(5)

```
cbkadal@osp:~/git/os211/TXT$ ls -al
total 24
drwxr-xr-x 2 cbkadal cbkadal 4096 Mar  5 13:18 .
drwxr-xr-x 9 cbkadal cbkadal 4096 Mar  3 14:38 ..
-rw-r--r-- 1 cbkadal cbkadal 1171 Mar  5 13:19 mylog.txt
-rw-r--r-- 1 cbkadal cbkadal 3147 Mar  5 13:19 mypubkey.txt
-rw-r--r-- 1 cbkadal cbkadal  491 Mar  5 13:19 myrank.txt
-rw-r--r-- 1 cbkadal cbkadal  453 Mar  5 13:19 myscript.sh

cbkadal@osp:~/git/os211/TXT$ bash myscript.sh 
rm -f SHA256SUM SHA256SUM.asc
sha256sum my*.txt my*.sh > SHA256SUM
sha256sum -c SHA256SUM
mylog.txt: OK
mypubkey.txt: OK
myrank.txt: OK
myscript.sh: OK
gpg -o SHA256SUM.asc -a -sb SHA256SUM
gpg --verify SHA256SUM.asc SHA256SUM
gpg: Signature made Fri 05 Mar 2021 13:19:16 WIB
gpg:                using RSA key 56754A8214D01B20B97BF5EF078CA2C2F3F22F37
gpg: Good signature from "Cicak Bin Kadal (CBK) <cbk@dummy>" [ultimate]

cbkadal@osp:~/git/os211/TXT$ git pull
Already up to date.

cbkadal@osp:~/git/os211/TXT$ git add -A

cbkadal@osp:~/git/os211/TXT$ git commit -m "OS211 cbkadal TXT"
[master 5b0e708] OS211 cbkadal TXT
 6 files changed, 168 insertions(+)
 create mode 100644 TXT/SHA256SUM
 create mode 100644 TXT/SHA256SUM.asc
 create mode 100644 TXT/mylog.txt
 create mode 100644 TXT/mypubkey.txt
 create mode 100644 TXT/myrank.txt
 create mode 100644 TXT/myscript.sh

cbkadal@osp:~/git/os211/TXT$ git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 6 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 4.32 KiB | 4.32 MiB/s, done.
Total 9 (delta 1), reused 2 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:cbkadal/os211.git
   8fd6980..5b0e708  master -> master

cbkadal@osp:~/git/os211/TXT$ ls -al
total 32
drwxr-xr-x 2 cbkadal cbkadal 4096 Mar  5 13:19 .
drwxr-xr-x 9 cbkadal cbkadal 4096 Mar  3 14:38 ..
-rw-r--r-- 1 cbkadal cbkadal 1171 Mar  5 13:19 mylog.txt
-rw-r--r-- 1 cbkadal cbkadal 3147 Mar  5 13:19 mypubkey.txt
-rw-r--r-- 1 cbkadal cbkadal  491 Mar  5 13:19 myrank.txt
-rw-r--r-- 1 cbkadal cbkadal  453 Mar  5 13:19 myscript.sh
-rw-r--r-- 1 cbkadal cbkadal  310 Mar  5 13:19 SHA256SUM
-rw-r--r-- 1 cbkadal cbkadal  833 Mar  5 13:19 SHA256SUM.asc

cbkadal@osp:~/git/os211/TXT$ 

```

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](CBKadal.md)
[NEXT](CBKadal3.md)

