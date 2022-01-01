# DYMO SDK for Linux – CUPS drivers

```
Revision 1 - May 31, 2006
Revision 2 – June 20, 2008
Revision 3 – July 10, 2009
Revision 4 – November 10, 2011
Revision 5 – March 25, 2012
```
## Overview
The DYMO SDK for Linux contains Linux drivers for the LabelWriter and LabelManager product lines. The drivers conform to the CUPS (Common UNIX Printing System) standard. The SDK also includes documentation, driver source code and examples of use.



## Requirements
The drivers were tested with CUPS version 1.4.6 and 1.5.0.


## Operating system
The drivers have been tested under following Linux distributions so far and will work on most Linux distributions with CUPS as long as the CUPS package dependencies are met.
* Ubuntu 10.04
* Ubuntu 11.04
* OpenSUSE 11.4
* OpenSUSE 12.1

**Note:** The printing is very slow on Ubuntu 11.10 since the ‘usb’ backend of CUPS has no backchannel support! This problem will be fixed with Ubuntu 12.04.

The drivers will work under other operating systems where CUPS is running. For example, other UNIX systems like Sun Solaris, AIX, BSD, Macintosh OS X, etc.  

## License
Drivers are provided under the GPL license version 2.  See the full text of the license in the LICENSE file.


## DYMO Products Supported

The following products are supported:
* LabelWriter 450
* LabelWriter 450 Turbo
* LabelWriter 450 Twin Turbo
* LabelWriter 450 DUO
* LabelWriter 4XL
* LabelWriter 400
* LabelWriter 400 Turbo
* LabelWriter 400 DUO
* LabelWriter 400 Twin Turbo
* LabelWriter 310 (models 90966, 93029 & 93034 **ONLY**)
* LabelWriter 315 (model 90975 **ONLY**)
* LabelWriter 320 (models 90892, 93031 & 93036 **ONLY**)
* LabelWriter 330 (model 90891 & 93037 USB **ONLY**)
* LabelWriter 330 Turbo (models 90884, 93033 & 93038, USB **ONLY**)
* LabelManager 500TS
* LabelMANAGER 450
* LabelMANAGER PC II
* LabelPOINT 350

These products should work with direct USB or serial port connections as well as shared over the network from other Linux or Windows machine.

The following products can work only when shared over the network from a Windows machine. This is due to limitations in the USB support in these printers – Linux USB support only recognizes fully compliant USB devices.
* LabelMANAGER 400
* LabelMANAGER PC

## Support Level
Drivers are provided AS-IS with NO WARRANTIES, with basic e-mail support only. 

## Driver version
Latest driver version is 1.5.0.5.


## SDK Contents
- Drivers in source form
- Installation script 
- Command line driven sample programs
1. **paper_list** - displays all paper sizes with dimensions and printable areas for a given printer. Uses only CUPS API.
2. **paper_bounds** - prints a bounding rectangle for all papers. Uses CUPS API and Cairo graphics library.
3. **test_label** - prints a test label contained aligned text, image, photo,	rectangle, lines. Shows how 3-party application can create a label and print it.
