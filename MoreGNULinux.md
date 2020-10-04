---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](Welcome2GNULinux.md)
[NEXT](CBKadal.md)

# More Gnu/Linux

<span style="color:red; font-weight:bold; font-size:larger;">
You need an editor for this page. Preferable, the vi (visual) editor.
</span>


<br>
## Substitute User/su (default root)
```
su -
```
<br>
## Add (a) user dummy
```
adduser dummy
```
<br>
<img src="pictures/LK-OSP-00.jpg" width="960">
<br>
<br>
## Substitute user dummy
```
pwd
su - dummy
```
### Testing home directory user dummy and then "exit"
```
pwd
exit
```
<img src="pictures/LK-OSP-01.jpg" width="960">
<br>
<br>
## Create/Edit your first file: "**.bash_aliases**"
* Use your favorite editor (vi) to add this following TEXT to file .bash_aliases.
<br>
<img src="pictures/LK-OSP-02.jpg" width="960">

```
alias cl='clear'
alias h='history'  
alias mv='mv -i'  
alias rm='rm -i'  
alias sss='. ~/.profile'
alias sbadak="ssh -p 6023 cbkadal@localhost"
alias tunnel='ssh -L 6023:badak.cs.ui.ac.id:22 cbkadal@kawung.cs.ui.ac.id'
alias rsyncDocs="  rsync -auv --delete -e 'ssh -p 6023' cbkadal@localhost:/extra/Docs/   /home/cbkadal/extra/Docs/"
alias rsyncDemos=" rsync -auv --delete -e 'ssh -p 6023' cbkadal@localhost:/extra/Demos/  /home/cbkadal/extra/Demos/"
alias rsyncSlides="rsync -auv --delete -e 'ssh -p 6023' cbkadal@localhost:/extra/Slides/ /home/cbkadal/extra/Slides/"
gitstat() {
   git rev-parse --is-inside-work-tree &> /dev/null
   [ "$?" == "0" ] && git status
   ls -aF
   printf "ZCZCNNNN ==== %s ===== PWD:%s\n" "$date)" $(pwd)
}
chktoken() {
    [ -z $1 ] && { 
        echo "Usage: chktoken <token>"
        echo "Is $USER your GitHub Account? If not, please cleate a new user name"
        return -1
    } || [ $1 == 0 ] && {
        echo "0"
        return 0
    } || [ $1 == 1 ] && {
        echo "$USER"
        return 0
    } || {
        STAMP=$(date +%M%S)
        echo "$STAMP-$(echo $STAMP$USER$1 | sha1sum  | cut -c1-4 | tr '[:lower:]' '[:upper:]'  )"
        return 0
    }
}
export EDITOR=/usr/bin/vi
export HISTSIZE=2000
export HISTFILESIZE=2000 
```
<br>
<br>
## Testing ".bash_aliases"
### "h" is an alias for "history"
```
h
source ~/.profile
h
```

<img src="pictures/LK-OSP-04.jpg" width="960">

<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://osp4diss.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/osp4diss/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](Welcome2GNULinux.md)
[NEXT](CBKadal.md)
<br>

