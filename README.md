# Zeek File Carving 

## Purpose
Zeek module which conducts file carving on specific MIME detected entities in sessions.

## Installation/Upgrade

This script was tested using Zeek 3.0.11

This is easiest to install through the Zeek package manager::

	zkg refresh
	zkg install https://github.com/nturley3/zeek-file-sniff

If you need to upgrade the package::

	zkg refresh
	zkg upgrade https://github.com/nturley3/zeek-file-sniff

See the [Zeek Package Manager Docs](https://docs.zeek.org/projects/package-manager/en/stable/quickstart.html) for more information.

## Configuration

The config.zeek file gives Zeek admins the option to check only local networks.
Module will automatically generate the notice logs.


## Generated Outputs

This script generates the following notices: 

| Notice Name | Description |
| -- | -- |
| FileSniff::x-php | File carve on PHP script |
| FileSniff::x-shellscript | File carve on shell script |
| FileSniff::x-python | File carve on Python script |
| FileSniff::x-perl | File carve on Perl script |


## Usage

Attackers often attempt to place scripts on a targeted machine. By logging the scripts, a security analyst can review them to determine if they are malicious. Ideally the extracted scripts can be fed into an antivirus engine for further analysis.

Tags: Alert, Threat Hunting, Hygiene

## About

Written by [@nturley3](https://github.com/nturley3).