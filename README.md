chkdel
======

The `chkdel` program is a simple tool written in Python which aim to check for running processes using files that have
been deleted or replaced on the filesystem.

It has been developed as a simplified alternative to the `checkrestart` tool provided under GNU/Linux Debian by the
_debian-goodies_ package.

Its code is available at [Github][0], and is licensed under the terms of the [BSD license][1].

**Requirements:**

* Python 2.5+

**Usage:**

	$ chkdel -v
	PID: 23848
	Program: /usr/bin/python2.6
	Files:
	   /usr/lib/libssl.so.0.9.8
	Command:
	   python /usr/sbin/denyhosts --daemon --purge --config=/etc/denyhosts.conf --config=/etc/denyhosts.conf

	Found 1 process using deleted files
	1 distinct program:
	   /usr/bin/python2.6
	1 distinct file:
	   /usr/lib/libssl.so.0.9.8


[0]: http://github.com/vbatoufflet/chkdel
[1]: http://opensource.org/licenses/BSD-3-Clause
