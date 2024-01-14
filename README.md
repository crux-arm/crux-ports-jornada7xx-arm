# crux-ports-jornada7xx-arm

CRUX-ARM ports overlay for HP Jornada 710/720/728

> IMPORTANT NOTE:
>
> Native compilation to build some ports of this repository is discouraged given the limitations of this device.
> Instead it is preferable to use cross-compilation.
>
> For this reason you may find some ports which the Pkgfile file contains logic for detecting native or cross compilation.
>

To use these ports, download the `jornada7xx-arm.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/crux-arm/crux-ports-jornada7xx-arm/2.6/jornada7xx-arm.httpup
$ sudo ports -u jornada7xx-arm
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/jornada7xx-arm
prtdir /usr/ports/core-arm
prtdir /usr/ports/opt-arm
prtdir /usr/ports/xorg-arm
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
