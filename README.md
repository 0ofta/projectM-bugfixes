# projectM-bugfixes

Patch for projectM to fix text rendering bugs.

bugfixes-22.02.2015.patch

This package is made from the abs Arch Linux package. It is tested still working september 2016 ;)

Usage (for Arch Linux):

install abs with pacman:

$ sudo pacman -S abs

run abs to download repos:

$ sudo abs

copy the projectm folder from community repo:

$ cp -r /var/abs/community/projectm ~/destination-folder

edit the PKBUILD to include this patch, then make and install the package:

$ makepkg -s -i -c

Cheers
