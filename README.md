# Sloth

<img src="resources/sloth_icon.png" align="right" style="float: right; margin-left: 30px;">

Sloth is a Mac application that displays a list of all open files and sockets in use by all running applications on your system. This makes it easy to see which apps are using which files and sockets.

Sloth is a GUI built on top of the powerful [`lsof`](https://en.wikipedia.org/wiki/Lsof) command line tool. The output of `lsof` is parsed and shown in a searchable, filterable table view with some convenient user-friendly functionality such as revealing files in the Finder, killing a file's owning process, displaying file info, filtering by volumes, and so on. See screenshots.

## Download

* [Download Sloth 2.2](http://sveinbjorn.org/files/software/sloth.zip) (~0.5 MB, Intel 64-bit, 10.8 or later)

## Screenshots

<img src="resources/sloth_screenshot2.jpg" align="center">

<img src="resources/sloth_screenshot1.jpg" align="center">

## Version history

## 07/03/2018 - Version 2.2

* Now defaults to excluding process binaries, shared libraries and current working directories in listing
* DNS and port name lookup now disabled by default for faster execution (can be enabled in Preferences)
* Info Panel now displays file access mode and process owner
* New sort option: User ID
* Info Panel now shows IP socket protocol and version
* New Preferences window
* New high-resolution pipe and socket icons
* Fixed bug where sort settings were not respected on launch

### 12/02/2018 - Version 2.1

* Copying a file path now creates a file representation in clipboard in addition to text
* File paths are now red in colour if selected file does not exist at path
* Uniform Type Identifier is now used to identify app bundles instead of .app suffix
* Fixed issue with Info Window's handling of moved or non-existent files
* Minor interface refinements

### 01/10/2017 - Version 2.0

* New Volumes filter
* New "Sort By" submenu under View in main menu
* Sorting by PID now correctly does numerical sort instead of alphabetic

### 07/06/2017- Version 1.9

* Files can now be dragged and dropped
* Cmd-F now focuses on filter field
* File representations can now be copied to the clipboard
* Cmd-double-click now reveals file in Finder
* Fixed various minor user interface bugs
* Fixed collapse all bug with Get Info window open
* New compact interface size option
* Fixed broken permissions display for non-bundle processes in Info window

### 03/05/2017 - Version 1.8

* Sloth is now code-signed
* QuickLook now works from Get Info panel
* Minor user interface improvements

### 17/06/2016 - Version 1.7

* New Info Panel for items
* Minor UI changes

### 24/02/2016 - Version 1.6

* Asynchronous refresh
* Much improved performance
* UI improvements
* New filtering options
* Smarter regex filtering
* Load results as root without restart
* Expanded sorting options
* Migrated project to ARC, modern Objective-C and XCode 7
* Substantial rewrite
* Now requires OS X 10.8 or later

### 08/07/2010 - Version 1.5

* Column sorting, column rearrangement
* Several bug fixes
* Copy/Drag and drop

### 29/05/2009 - Version 1.4

* Regular expression search filtering
* New "Relaunch as root" option
* Fixed bug in Mac OS X 10.5
* Now built for Mac OS X 10.4 or later

### 28/07/2006 - Version 1.3.1

* Released as a Universal Binary

### 05/03/2004 - Version 1.3

* Live update on search filter
* Sorting in columns now works
* Performance improvements
* The timed update feature is non-functional for the time being
* Lots of code replaced by Cocoa bindings thanks to Bill Bumgarner

### 27/02/2004 - Version 1.2

* Filter search field now counts all list fields when filtering
* Auto-refresh timer option
* Preferences for setting arbitrary lsof binary and kill signal type
* New application icon
* Added Icelandic and Japanese localizations

### 22/02/2004 - Version 1.1

* There is now a search field filter for entries in list. No type-in update.
* "Actions" menu with menu items and shortcuts for button actions

### 21/02/2004 - Version 1.0

## BSD License 

Copyright (C) 2004-2018 Sveinbjorn Thordarson <sveinbjornt@gmail.com>

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this
list of conditions and the following disclaimer in the documentation and/or other
materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors may
be used to endorse or promote products derived from this software without specific
prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.
