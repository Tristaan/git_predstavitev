Postavitev git "strežnika"
============
``` bash
    ssh user@XXX.XXX.XXX.XXX
    git init --bare ~/build/git_predstavitev.git
    exit #Izhod iz ssh-ja, naprej lokalno
```
Lokalna kopija
=============
## 1. način
``` bash
    git clone user@XXX.XXX.XXX.XXX:build/git_predstavitev.git
```

## 2. način (npr. če imamo že obstoječi projekt)
``` bash
    cd moj_projekt
    # git init
    git remote add origin user@XXX.XXX.XXX.XXX:build/git_predstavitev.git
    git push -u origin master # potisk sprememb v remote origin
```

