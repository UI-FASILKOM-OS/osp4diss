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
* No passphrase.

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
gpg: revocation certificate stored as '/home/cbkadal/.gnupg/openpgp-revocs.d/C13787F94073986F0FE39A4E6BE9DC2074F27BF1.rev'
public and secret key created and signed.

pub   rsa4096 2020-09-28 [SC] [expires: 2021-09-28]
      C13787F94073986F0FE39A4E6BE9DC2074F27BF1
uid                      Cicak Bin Kadal (CBK) <cbk@dummy>
sub   rsa4096 2020-09-28 [E] [expires: 2021-09-28]
```

<br>
## List the keys

```
cbkadal@osp:~$ gpg --list-keys
gpg: checking the trustdb
gpg: marginals needed: 3  completes needed: 1  trust model: pgp
gpg: depth: 0  valid:   1  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 1u
gpg: next trustdb check due at 2021-09-28
/home/cbkadal/.gnupg/pubring.kbx
--------------------------------
pub   rsa4096 2020-09-28 [SC] [expires: 2021-09-28]
      C13787F94073986F0FE39A4E6BE9DC2074F27BF1
uid           [ultimate] Cicak Bin Kadal (CBK) <cbk@dummy>
sub   rsa4096 2020-09-28 [E] [expires: 2021-09-28]

cbkadal@osp:~$ 
```
<br>
## Importing the Operating Systems public key
* Source: <https://osp4diss.vlsm.org/ETC/ospubkey.txt>

```
cbkadal@osp:~$ gpg --import ospubkey.txt 
gpg: key D0F5DBDD67DF6DDE: public key "Operating Systems (OS) <operatingsystems@vlsm.org>" imported
gpg: Total number processed: 1
gpg:               imported: 1
cbkadal@osp:~$ gpg --list-keys
/home/cbkadal/.gnupg/pubring.kbx
--------------------------------
pub   rsa4096 2020-09-28 [SC] [expires: 2021-09-28]
      C13787F94073986F0FE39A4E6BE9DC2074F27BF1
uid           [ultimate] Cicak Bin Kadal (CBK) <cbk@dummy>
sub   rsa4096 2020-09-28 [E] [expires: 2021-09-28]

pub   rsa4096 2020-02-13 [SC] [expires: 2021-02-12]
      B4507B533F7F22840BD8E93ED0F5DBDD67DF6DDE
uid           [ unknown] Operating Systems (OS) <operatingsystems@vlsm.org>
sub   rsa4096 2020-02-13 [E] [expires: 2021-02-12]

cbkadal@osp:~$
```
<br>
## Export Public Key "mypubkey.txt"

```
cbkadal@osp:~$ cd git/os202/TXT/
cbkadal@osp:~/git/os202/TXT$ gpg -o mypubkey.txt --armor --export C13787F94073986F0FE39A4E6BE9DC2074F27BF1
cbkadal@osp:~/git/os202/TXT$ ls -al
total 24
drwxr-xr-x 2 cbkadal cbkadal 4096 Sep 28 23:25 .
drwxr-xr-x 6 cbkadal cbkadal 4096 Sep 28 22:12 ..
-rw-r--r-- 1 cbkadal cbkadal  630 Sep 28 18:11 mylog.txt
-rw-r--r-- 1 cbkadal cbkadal 3147 Sep 28 23:25 mypubkey.txt
-rw-r--r-- 1 cbkadal cbkadal  119 Sep 28 21:35 myrank.txt
-rw-r--r-- 1 cbkadal cbkadal  419 Sep 28 22:06 myscript.sh
cbkadal@osp:~/git/os202/TXT$
```
<br>
## Generate SHA256SUM and SHA256SUM.asc

```
cbkadal@osp:~/git/os202/TXT$ bash myscript.sh 
sha256sum mylog.txt mypubkey.txt myrank.txt myscript.sh > SHA256SUM
sha256sum -c SHA256SUM
mylog.txt: OK
mypubkey.txt: OK
myrank.txt: OK
myscript.sh: OK
gpg -o SHA256SUM.asc -a -sb SHA256SUM
gpg --verify SHA256SUM.asc SHA256SUM
gpg: Signature made Mon 28 Sep 2020 11:26:55 PM WIB
gpg:                using RSA key C13787F94073986F0FE39A4E6BE9DC2074F27BF1
gpg: Good signature from "Cicak Bin Kadal (CBK) <cbk@dummy>" [ultimate]
cbkadal@osp:~/git/os202/TXT$ ls -al
total 32
drwxr-xr-x 2 cbkadal cbkadal 4096 Sep 28 23:26 .
drwxr-xr-x 6 cbkadal cbkadal 4096 Sep 28 22:12 ..
-rw-r--r-- 1 cbkadal cbkadal  630 Sep 28 18:11 mylog.txt
-rw-r--r-- 1 cbkadal cbkadal 3147 Sep 28 23:25 mypubkey.txt
-rw-r--r-- 1 cbkadal cbkadal  119 Sep 28 21:35 myrank.txt
-rw-r--r-- 1 cbkadal cbkadal  419 Sep 28 22:06 myscript.sh
-rw-r--r-- 1 cbkadal cbkadal  310 Sep 28 23:26 SHA256SUM
-rw-r--r-- 1 cbkadal cbkadal  833 Sep 28 23:26 SHA256SUM.asc
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
[PREV](CBKadal.md)
[NEXT](CBKadal3.md)

