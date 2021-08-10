# msk_kiss
msk_kiss: My personal KISS repository

Don't take this is an accurate representation of my git commiting skills; due to
the highly informal nature of this, the commit history will be even sloppier than
usual. Also, *do not expect high-quality packages*. The 100% first priority is 
packaging things for _myself_, so I would recommend going in with the mindset of 
"this package I found isn't going to build". At worst, you'll have a starting
point for making your own package, and at best, you'll be pleasantly surprised with
a working one.

## Notes
- sbase
	- The community sbase package but forked to keep sed.
	The original unlinks it.
- clipmenu-git (you need to use a few kiss alternatives to busybox)
	- procps-ng for /usr/bin/pgrep
	- util-linux for /usr/bin/flock
- qutebrowser-git (finally)
	- Credit to https://github.com/sdsddsd1, I used their packages as a base for qutebrowser and its dependencies
	- The build file removes the dbus dependency, but also breaks support for web notifications (which I don't need)
- gomuks-git
	- I get a long set of "permission denied" errors for deleting cached files at the end of the build, and am not sure what's causing it - if you're familiar with Go, please offer some advice
- w3l-git
	- It also depends on termcap, which I wasn't able to successfully package.
	- ```sh
	curl -O http://ftp.gnu.org/gnu/termcap/termcap-1.3.1.tar.gz
	tar xf termcap-1.3.1.tar.gz
	rm termcap-1.3.1.tar.gz
	cd termcap-1.3.1
	./configure
	su -c "make install"
	```
- elinks
	- This package was made by testuser, not me! It's only here to ensure that I
	don't lose it between e.g. multiple installs.
- libmupdf
	- Upstream has some sort of issue ATM.
- lynx
	- Use OpenSSL instead of LibreSSL.
- falkon
	- wayland --> xorg

## Scripts (kiss extensions)
- kiss-new - a fork that adds some 'default(?)' commands to the build file
	- if using, make sure /path/to/msk_kiss/scripts is before /usr/bin/ in your $PATH
- kiss-source - quickly output the sources of a package
- kiss-hook - you should probably just ignore this

## My kernel configuration for some hardware
- hp-elitebook-8470p
