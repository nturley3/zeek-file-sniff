Zeek File Carving 
======================

Zeek module which conducts file carving on specific MIME detected entities
in sessions.

Installation/Upgrade
------------

This is easiest to install through the Bro package manager::

	zkg refresh
	zkg install https://github.com/nturley3/zeek-file-sniff

If you need to upgrade the package::

	zkg refresh
	zkg upgrade https://github.com/nturley3/zeek-file-sniff

Usage
-----

This script generates the following notices: 

**FileSniff::x-php** - File carve on PHP script

**FileSniff::x-shellscript** - File carve on shell script

**FileSniff::x-python** - File carve on Python script

**FileSniff::x-perl** - File carve on Perl script

