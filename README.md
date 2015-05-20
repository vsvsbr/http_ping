# About http_ping
Perl script found in http://prefetch.net/code/index.html

Author: Matty < matty91 at gmail dot com >

Current Version: 1.1

# Purpose
  Reports latency between a web server and a given host

# License
This program is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the
Free Software Foundation; either version 2, or (at your option) any
later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, 59 Temple Place - Suite 330, Boston, MA 02111-1307, USA.

# Installation
Install Net::HTTP, and copy the shell script to a suitable location

# Usage
Usage: http-ping.pl [ -s server ] [ -p port ] [ -d delay ] [ -u uri ] [ -h ]

## Example
```
  $ ./http-ping.pl -s www.prefetch.net -p 80 -d 5 -u /index.html
   Querying HTTP server www.prefetch.net:80 every 5 seconds (Ctrl-C to stop):
      Mon Nov 29 18:09:59 2004: TCP Connection Time=0.052s HTTP GET Time=0.051s [Normal Delay]
      Mon Nov 29 18:10:04 2004: TCP Connection Time=0.036s HTTP GET Time=0.052s [Normal Delay]
      Mon Nov 29 18:10:09 2004: TCP Connection Time=0.034s HTTP GET Time=0.052s [Normal Delay]
```
