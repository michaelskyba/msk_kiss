# msk_kiss
msk_kiss: My personal KISS repository

Don't take this is an accurate representation of my git commiting skills; due to
the highly informal nature of this, the commit history will be even sloppier than
usual. Also, *do not expect high-quality packages*. The 100% first priority is 
packaging things for _myself_, so I would recommend going in with the mindset of 
"this package I found isn't going to build". At worst, you'll have a starting
point for making your own package, and at best, you'll be pleasantly surprised with
a working one.

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
- bombadillo-git
- pyqt5 (I think)
- pyqtwebengine
- qutebrowser-git (finally)
	- Credit to https://github.com/sdsddsd1, I used their packages as a base for qutebrowser and its dependencies
	- The build file removes the dbus dependency, but also breaks support for web notifications (which I don't need)
- olm-git
- gomuks-git
	- I get a long set of "permission denied" errors for deleting cached files at the end of the build, and am not sure what's causing it - if you're familiar with Go, please offer some advice
- btpd-git

Forks with misc fixes
- msmtp (openssl)
- lynx (openssl)
- libmupdf (temporary failure)

## Exports (binary packages):
- llvm (backup)
- nodejs (backup)
- qt5-webengine (new)

## Scripts (kiss extensions)
- kiss-new - a fork that adds some 'default(?)' commands to the build file
	- if using, make sure /path/to/msk_kiss/scripts is before /usr/bin/ in your $PATH
- kiss-source - quickly output the sources of a package
- kiss-hook - you should probably just ignore this

## My kernel configuration Tor some hardware
- hp-elitebook-8470p
