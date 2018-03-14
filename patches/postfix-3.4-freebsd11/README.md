# What?
Minor patch to enable compilation of vanilla Postfix 3.4 sources on FreeBSD 11.
Solves the following issue:
```
ATTENTION:
ATTENTION: Unknown system type: FreeBSD 11.1-RELEASE-p4
ATTENTION:
*** Error code 1
```

# How?
```
$ tar -xf postfix-3.4-20180222.tar.gz
$ cd postfix-3.4-20180222
$ patch -p2 < /path/to/postfix-3.4-20180222.freebsd.patch
$ make
```
