[![Build Status](https://travis-ci.org/simoncadman/CUPS-Cloud-Print.png)](https://travis-ci.org/simoncadman/CUPS-Cloud-Print)

INTRODUCTION
============
Google Cloud Print driver for CUPS, allows printing to printers hosted on Google Cloud Print. 

INSTALLATION
============

PACKAGE INSTALL ( Recommended )
================================

The recommended way to install CUPS Cloud Print is using your package manager, please see http://ccp.niftiestsoftware.com/ for installation 
instructions.

SOURCE INSTALL
==============

Clone the git repo:

git clone git://github.com/simoncadman/CUPS-Cloud-Print.git

cd CUPS-Cloud-Print/
./configure
make install

Follow configuration below.

CONFIGURATION
=============

Run /usr/lib/cloudprint-cups/setupcloudprint.py ( or /usr/local/lib/cloudprint-cups/setupcloudprint.py ) and either allow it to add all 
Cloud Print printers at once, or say 'N', and add manually:

Add a new printer ( via http://127.0.0.1:631 or usual interface ) as a 'Google Cloud Print' network printer. Select the 'Make' as Google, and 'Model' as Cloud Print.
Supply the connection name as a simple URI pointing to the printer you want to setup, you can obtain a list of URIs from 
/usr/lib/cloudprint-cups/listcloudprinters.py ( or /usr/local/lib/cloudprint-cups/listcloudprinters.py ) :
  
Print a test page, to confirm it is working.

Assuming the test page prints correctly, installation is complete.


Copyright and Trademark Information
===================================

Printer part of icon from Oxygen Iconset ( http://www.oxygen-icons.org/ ) and licenced under GNU LGPL v3 ( http://www.gnu.org/licenses/lgpl.html ).

Software and icon are copyright Simon Cadman and licenced under GNU GPL v3 ( http://www.gnu.org/licenses/gpl.html ).

Google is a trademark of Google Inc, and the software is unaffiliated with Google in any way.

CUPS and the CUPS logo are trademarks of Apple Inc. CUPS is copyright Apple Inc.