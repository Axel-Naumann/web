---
layout: releases
version: 6.12/06
release_date: 2018-02-09
state:

toc: true
toc_sticky: true
sidebar:
  nav: "download"
---

## Highlights

New: support for C++17 with GCC 7.3.

## Release Notes

The release notes for this release can be found [here](https://root.cern.ch/doc/v612/release-notes.html#release-6.1206).

## Source distribution

| Platform       | Files | Size |
|-----------|-------|-----|
| source | [root_v6.12.06.source.tar.gz](https://root.cern.ch/download/root_v6.12.06.source.tar.gz) | 155M |


## Binary distributions

| Platform       | Files | Size |
|-----------|-------|-----|
| CentOS Cern 7 gcc4.8 | [root_v6.12.06.Linux-centos7-x86_64-gcc4.8.tar.gz](https://root.cern.ch/download/root_v6.12.06.Linux-centos7-x86_64-gcc4.8.tar.gz) | 134M |
| Linux fedora26 gcc7.2 | [root_v6.12.06.Linux-fedora26-x86_64-gcc7.2.tar.gz](https://root.cern.ch/download/root_v6.12.06.Linux-fedora26-x86_64-gcc7.2.tar.gz) | 121M |
| Linux fedora27 gcc7.2 | [root_v6.12.06.Linux-fedora27-x86_64-gcc7.2.tar.gz](https://root.cern.ch/download/root_v6.12.06.Linux-fedora27-x86_64-gcc7.2.tar.gz) | 121M |
| Ubuntu 14 gcc4.8 | [root_v6.12.06.Linux-ubuntu14-x86_64-gcc4.8.tar.gz](https://root.cern.ch/download/root_v6.12.06.Linux-ubuntu14-x86_64-gcc4.8.tar.gz) | 120M |
| Ubuntu 16 gcc5.4 | [root_v6.12.06.Linux-ubuntu16-x86_64-gcc5.4.tar.gz](https://root.cern.ch/download/root_v6.12.06.Linux-ubuntu16-x86_64-gcc5.4.tar.gz) | 121M |
| Ubuntu 17 gcc7.2 | [root_v6.12.06.Linux-ubuntu17-x86_64-gcc7.2.tar.gz](https://root.cern.ch/download/root_v6.12.06.Linux-ubuntu17-x86_64-gcc7.2.tar.gz) | 126M |
| OsX 10.12 clang90 | [root_v6.12.06.macosx64-10.12-clang90.dmg](https://root.cern.ch/download/root_v6.12.06.macosx64-10.12-clang90.dmg) | 125M |
| OsX 10.12 clang90 | [root_v6.12.06.macosx64-10.12-clang90.tar.gz](https://root.cern.ch/download/root_v6.12.06.macosx64-10.12-clang90.tar.gz) | 125M |
| OsX 10.13 clang90 | [root_v6.12.06.macosx64-10.13-clang90.dmg](https://root.cern.ch/download/root_v6.12.06.macosx64-10.13-clang90.dmg) | 127M |
| OsX 10.13 clang90 | [root_v6.12.06.macosx64-10.13-clang90.tar.gz](https://root.cern.ch/download/root_v6.12.06.macosx64-10.13-clang90.tar.gz) | 125M |



## Installations in CVMFS

Standalone installations with minimal external dependencies are available at:
~~~
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-mac1012-clang90-opt
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-fedora26-gcc72-opt
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-fedora27-gcc72-opt
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-ubuntu14-gcc48-opt
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-ubuntu16-gcc54-opt
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-centos7-gcc48-opt
/cvmfs/sft.cern.ch/lcg/app/releases/ROOT/6.12.06/x86_64-mac1013-clang90-opt
~~~


## Git

The entire ROOT source can be obtained from our public Git repository:

~~~
git clone http://github.com/root-project/root.git
~~~
The release specific tag can be obtained using:
~~~
cd root
git checkout -b v6-12-06 v6-12-06
~~~

