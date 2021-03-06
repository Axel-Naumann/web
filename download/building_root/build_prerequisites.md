---
title: Prerequisites
layout: single
sidebar:
  nav: "download"
toc: true
toc_sticky: true
---


Below are the required packages listed that must be installed on the various platforms to configure and build ROOT.
<br>If more advanced ROOT plugins are required look at the `cmake` or `./configure` output and add the desired third
party packages before configuring and building ROOT again.

- [Fedora family](#fedora-18-19-and-20-scientific-linux-5-6-centos-6-7)
- [Ubuntu family](#ubuntu-10-12--14-and-16)
- [OpenSUSE family](#opensuse-10-11)
- [Mac OS X family](#macos-x)
- [Windows family](#windows)
- [AIX family](#aix-5-6-and-7)

## Fedora 18, 19 and 20; Scientific Linux 5, 6; CentOS 6, 7

*   **git:** for /usr/bin/git
*   **make:** for /usr/bin/make
*   **cmake:** for /usr/bin/cmake
*   **gcc-c++:** for  for /usr/bin/g++ (ROOT 6 requires g++ 4.8 or clang 3.4; for SLC5/SLC6)
*   **gcc:** for /usr/bin/gcc
*   **binutils:** for /usr/bin/ld
*   **libX11-devel:** for usr/include/X11/Xlib.h and for /usr/lib/libX11.so
*   **libXpm-devel:** for /usr/include/X11/xpm.h and for /usr/lib/libXpm.so
*   **libXft-devel:** for /usr/include/X11/Xft/Xft.h and for /usr/lib/libXft.so
*   **libXext-devel:** for /usr/include/X11/extensions/shape.h and for /usr/lib/libXext.so
*   **python:**  (ROOT6 requires version >= 2.7)
*   **redhat-lsb-core:**   needed by some tests (tutorials) using lsb_release and some CDash scripts

### Most common optional packages

*   **gcc-gfortran:** for /usr/bin/gfortran
*   **openssl-devel:** for /usr/include/openssl/pem.h and /usr/lib/libssl.so and /usr/lib/libcrypto.so
*   **pcre-devel:** for /usr/bin/pcre-config
*   **mesa-libGL-deve**l: for /usr/include/GL/gl.h and for /usr/lib[64]/libGL.so
*   **mesa-libGLU-devel**: for /usr/include/GL/glu.h and for /usr/lib[64]/libGLU.so
*   **glew-devel (may need enabling of the [EPEL](http://fedoraproject.org/wiki/EPEL) additional software repository)**: for /usr/include/GL/glew.h and for /usr/lib[64]/libGLEW.so
*   **ftgl-devel:** for /usr/bin/pkg-config
*   **mysql-devel:** for /usr/bin/mysql_config
*   **fftw-devel:** for /usr/include/fftw3.h and for /usr/lib/libfftw3.so
*   **cfitsio-devel:** for /usr/include/fitsio2.h and for /usr/lib/libcfitsio.so
*   **graphviz-devel:** for /usr/include/graphviz/gvc.h and for /usr/lib/libgvc.so
*   **avahi-compat-libdns_sd-devel:** for /usr/include/dns_sd.h and for /usr/lib/libdns_sd.so
*   **libldap-dev:** for /usr/include/ldap.h and for /usr/lib/libldap.so
*   **python-devel:** for /usr/include/python2.7/Python.h and for /usr/lib/libpython2.7.so
*   **python-numpy-devel:** needed for PyMVA
*   **libxml2-devel:** for /usr/bin/xml2-config
*   **gsl-static:** for /usr/include/gsl/gsl_version.h and for /usr/lib/libgsl.a. On Fedora 16 use **gsl-devel**.
*   **r-base:** needed for R bindings. In addition R packages **Rcpp** and **RInside** need to be installed.

Use `yum install _package_` or use the graphical "Add/Remove Software" program.

**Required packages**

```
   sudo yum install git cmake gcc-c++ gcc binutils \
   libX11-devel libXpm-devel libXft-devel libXext-devel
```


**Optional packages**

```
   sudo yum install gcc-gfortran openssl-devel pcre-devel \
   mesa-libGL-devel mesa-libGLU-devel glew-devel ftgl-devel mysql-devel \
   fftw-devel cfitsio-devel graphviz-devel \
   avahi-compat-libdns_sd-devel libldap-dev python-devel \
   libxml2-devel gsl-static
```

## Ubuntu 10, 12 , 14 and 16

*   **git:** for /usr/bin/git
*   **dpkg-dev**  for dpkg-architecture (needed by configure to locate system libraries starting from 11)
*   **cmake:** for /usr/bin/cmake
*   **g++:** for /usr/bin/g++  (ROOT 6 requires g++ 4.8 or clang 3.4  for how to install g++ 4.8 on Ubuntu 12 see [ubuntuhandbook](http://ubuntuhandbook.org/index.php/2013/08/install-gcc-4-8-via-ppa-in-ubuntu-12-04-13-04/){:target="_blank"})
*   **gcc:** for /usr/bin/gcc
*   **binutils:** for /usr/bin/ld
*   **libx11-dev:** for usr/include/X11/Xlib.h and for /usr/lib/libX11.so
*   **libxpm-dev:** for /usr/include/X11/xpm.h and for /usr/lib/libXpm.so
*   **libxft-dev:** for /usr/include/X11/Xft/Xft.h and for /usr/lib/libXft.so
*   **libxext-dev:** for /usr/include/X11/extensions/shape.h and for /usr/lib/libXext.so
*   **libpng:** png library
*   **libjpeg:** jpeg library
*   **python:** (ROOT6 requires version >= 2.7)

### Most common optional packages

*   **gfortran:** for /usr/bin/gfortran
*   **openssl-dev** or **libssl-dev:** for /usr/include/openssl/pem.h and /usr/lib/libssl.so and /usr/lib/libcrypto.so
*   **libpcre3-dev:** for /usr/bin/pcre-config
*   **xlibmesa-glu-dev:** for /usr/include/GL/gl.h and for /usr/lib/libGL.so
*   **libglew1.5-dev:** for /usr/include/GL/glew.h and for /usr/lib/libGLEW.so
*   **libftgl-dev:** for /usr/bin/pkg-config
*   **libmysqlclient-dev:** for /usr/bin/mysql_config
*   **libfftw3-dev:** for /usr/include/fftw3.h and for /usr/lib/libfftw3.so
*   **libcfitsio-dev:** for /usr/include/fitsio2.h and for /usr/lib/libcfitsio.so
*   **graphviz-dev:** for /usr/include/graphviz/gvc.h and for /usr/lib/libgvc.so
*   **libavahi-compat-libdnssd-dev:** for /usr/include/dns_sd.h and for /usr/lib/libdns_sd.so
*   **libldap2-dev:** for /usr/include/ldap.h and for /usr/lib/libldap.so
*   **python-dev:** for /usr/include/python2.7/Python.h and for /usr/lib/libpython2.7.so
*   **python-numpy-dev:** needed for PyMVA
*   **libxml2-dev:** for /usr/bin/xml2-config
*   **libkrb5-dev:** for /usr/include/krb5.h and for /usr/lib/libkrb5.so
*   **libgsl0-dev:** for /usr/include/gsl/gsl_version.h and for /usr/lib/libgsl.a
*   **libqt4-dev:** for /usr/include/qt4/Qt/qglobal.h and for /usr/lib/libQtCore.so
*   **r-base:** needed for R bindings. In addition R packages **Rcpp** and **RInside** need to be installed.

Use `sudo apt-get install _package_` or use the graphical "Synaptic Package Manager" program.

**Required packages**

```
   sudo apt-get install git dpkg-dev cmake g++ gcc binutils libx11-dev libxpm-dev \
   libxft-dev libxext-dev
```

**Optional packages**

```
   sudo apt-get install gfortran libssl-dev libpcre3-dev \
   xlibmesa-glu-dev libglew1.5-dev libftgl-dev \
   libmysqlclient-dev libfftw3-dev libcfitsio-dev \
   graphviz-dev libavahi-compat-libdnssd-dev \
   libldap2-dev python-dev libxml2-dev libkrb5-dev \
   libgsl0-dev libqt4-dev
```

## OpenSUSE 10, 11

*   **git:** for /usr/bin/git
*   **bash:** for /bin/bash
*   **cmake:** for /usr/bin/cmake
*   **gcc-c++:** for /usr/bin/g++
*   **gcc:** for /usr/bin/gcc
*   **binutils:** for /usr/bin/ld
*   **xorg-x11-libX11-devel:** for /usr/include/X11/Xlib.h and for /usr/lib[64]/libX11.so
*   **xorg-x11-libXpm-devel:** for /usr/include/X11/xpm.h and for /usr/lib[64]/libXpm.so
*   **xorg-x11-devel:** for /usr/include/X11/Xft/Xft.h and for /usr/lib[64]/libXft.so
*   **xorg-x11-proto-devel:** for /usr/include/X11/extensions/shape.h
*   **xorg-x11-libXext-devel:** for /usr/lib[64]/libXext.so

### Most common optional packages

*   **gcc-fortran:** for /usr/bin/gfortran
*   **libopenssl-devel:** for /usr/include/openssl/pem.h and /usr/lib[64]/libssl.so and /usr/lib[64]/libcrypto.so
*   **pcre-devel:** for /usr/bin/pcre-config
*   **Mesa:** for /usr/include/GL/gl.h and for /usr/lib[64]/libGL.so
*   **glew-devel:** for /usr/include/GL/glew.h and for /usr/lib[64]/libGLEW.so
*   **pkg-config:** for /usr/bin/pkg-config
*   **libmysqlclient-devel:** for /usr/bin/mysql_config
*   **fftw3-devel:** for /usr/include/fftw3.h and for /usr/lib[64]/libfftw3.so
*   **libcfitsio-devel:** for /usr/include/libcfitsio0/fitsio2.h and for /usr/lib[64]/libcfitsio.so (not available on openSUSE 10)
*   **graphviz-devel:** for /usr/include/graphviz/gvc.h and for /usr/lib[64]/libgvc.so
*   **avahi-compat-mDNSResponder (on openSUSE 10), libdns_sd (on openSUSE 11):** for /usr/lib[64]/libdns_sd.so
*   **avahi-compat-mDNSResponder-devel:** for /usr/include/dns_sd.h
*   **openldap2-devel:** for /usr/include/ldap.h and for /usr/lib[64]/libldap.so
*   **python-devel:** for /usr/include/python2.7/Python.h and for /usr/lib[64]/libpython2.7.so
*   **python-numpy-devel:** needed for PyMVA
*   **libxml2-devel:** for /usr/bin/xml2-config
*   **krb5-devel:** for /usr/include/krb5.h and for /usr/lib[64]/libkrb5.so
*   **gsl-devel:** for /usr/include/gsl/gsl_version.h and for /usr/lib[64]/libgsl.a
*   **libqt4-devel:** for /usr/include/Qt/qglobal.h and for /usr/lib[64]/libQtCore.so
*   **r-base:** needed for R bindings.  In addition R packages **Rcpp** and **RInside** need to be installed.

Use `sudo zypper install _package_` or use the graphical "Software / Package Manager" in the "YaST2 Control Center" utility.

**Required packages**

```
   sudo zypper install git bash cmake gcc-c++ gcc binutils \
   xorg-x11-libX11-devel xorg-x11-libXpm-devel xorg-x11-devel \
   xorg-x11-proto-devel xorg-x11-libXext-devel
```

**Optional packages**

```
   sudo zypper install gcc-fortran libopenssl-devel \
   pcre-devel Mesa glew-devel pkg-config libmysqlclient-devel \
   fftw3-devel libcfitsio-devel graphviz-devel \
   libdns_sd avahi-compat-mDNSResponder-devel openldap2-devel \
   python-devel libxml2-devel krb5-devel gsl-devel libqt4-devel
```

## MacOS X

*   **Xcode developer package:** for make, g++, gcc, ld, etc.  Xcode is found on the MacOS X installation DVD or in the Mac App store.
    install command line tools through the XCode preferences and/or running in a terminal  `xcode-select --install`
*   **[Xquartz](http://xquartz.macosforge.org/){:target="_blank"}:** for the X11 server (not needed in case the version with Cocoa native backend is build)
*   Other dependencies can be installed from [MacPorts](http://www.macports.org/){:target="_blank"}

### Most common optional packages

*   **gcc 4.x from [MacPorts](http://www.macports.org){:target="_blank"}:** for /opt/local/bin/gfortran
    or alternatively use this [gfortran.dmg](http://r.research.att.com/tools/){:target="_blank"}

Alternatively ROOT can be installed directly from [MacPort](http://www.macports.org){:target="_blank"} with the command:

```
sudo port install root
```

## Windows

If you are using Windows make sure you have installed Microsoft Visual C++ (e.g., the
[no-cost edition](http://www.microsoft.com/express/vc/){:target="_blank"}) plus `CMake`.
The `CMake` build will work directly **without the need** to install
[cygwin](http://cygwin.com){:target="_blank"} as it was required previously before the adaption of `CMake`.

> **Note:**

> Currently native Windows support for ROOT6 versions is not available.

## AIX 5, 6 and 7

*   **git:** for /usr/bin/git
*   **bash:** for /usr/bin/bash
*   **make:** for /usr/linux/bin/make
*   **pkg-config:** for fontconfig, freetype2, xft and xrender installation
*   **fontconfig:** for /usr/lib/libfontconfig.a
*   **fontconfig-devel:** for /usr/include/fontconfig
*   **freetype2:** for /usr/lib/libfreetype.a needed by xft
*   **freetype2-devel:** for /usr/include/freetype2
*   **libxml2:** for /usr/lib/libxml2.a
*   **libxml2-devel:** for /usr/bin/xml2-config
*   **xft:** for /usr/include/X11/Xft/Xft.h and /usr/lib/libXft.a
*   **xrender:** for /opt/freeware/include/X11/extensions/Xrender.h and /usr/lib/libXrender.a
*   **zlib:** for resolving dependencies
*   **zlib-devel:** for resolving dependencies
*   **expat:** for resolving dependencies

Use `rpm -Uvh _package_` to install the above packages from [AIX Toolbox for Linux Applications](http://www-03.ibm.com/systems/power/software/aix/linux/toolbox/alpha.html){:target="_blank"}. Subversion can be obtained from [collab.net](http://www.open.collab.net/downloads/community/){:target="_blank"}.