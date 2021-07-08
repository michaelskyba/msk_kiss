# msk_kiss
msk_kiss: My personal KISS repository

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
- py-sip4

## Exports (binary packages):
- llvm (backup)
- nodejs (backup)
- qt5-webengine (new)

## Scripts (kiss extensions)
- kiss-grep - search through installed repos for a package
- kiss-new - a fork that adds some 'default(?)' commands to the build file
	- if using, make sure /path/to/msk_kiss/scripts is before /usr/bin/ in your $PATH
- kiss-source - quickly output the sources of a package
