# msk_kiss
msk_kiss: My personal KISS repository

Don't take this is an accurate representation of my git commiting skills; due to the highly informal nature of this, the commit history will be even sloppier than usual.

## Currently 'working' packages (as of July 2021):
- xcape-git
- gettext
- snownews-git (I think)
- clipnotify-git
- clipmenu-git (you need to use a few kiss alternatives to busybox)
	- procps-ng for /usr/bin/pgrep
	- util-linux for /usr/bin/flock
- xbindkeys-git
- unclutter-xfixes-git
- aspell
- libxml-parser-perl
- intltool
- libqalculate
- py-sip
- mutt-wizard-git
    - I have added "lynx" and "urlview" as depencies, even though they are, in reality, optional
    - Modify the 'depends' file if they aren't required
- bombadillo-git
- pyqt5 (I think)
- gcolor3-git

## Exports (binary packages):
- llvm (backup)
- nodejs (backup)
- qt5-webengine (new)

## Scripts (kiss extensions)
- kiss-grep - search through installed repos for a package
- kiss-new - a fork that adds some 'default(?)' commands to the build file
	- if using, make sure /path/to/msk_kiss/scripts is before /usr/bin/ in your $PATH
- kiss-source - quickly output the sources of a package

## My kernel configuration for some hardware
- hp-elitebook-8470p
