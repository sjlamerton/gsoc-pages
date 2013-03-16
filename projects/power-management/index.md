---
layout: default
title: Power Management
---

## Implement support for power management under non-Windows platforms

wxWidgets has support for
[power events](http://docs.wxwidgets.org/trunk/classwx_power_event.html) but
it's implemented for Windows only right now and doesn't even work for Vista and
later systems right now, e.g. it's impossible to prevent the system from
suspending in this way (which was used until Windows XP) any more. The goal of
this project would be to update power management support for Windows Vista/7
(which is simple to do, see
[this thread](http://thread.gmane.org/gmane.comp.lib.wxwidgets.devel/120453))
and, most importantly, also implement them for Linux and/or OS X. This will
include devising an API which can be implemented on all platforms and actually
implementing it for Windows and at least one of Linux/OS X (and ideally both).

[**Difficulty:**](../project-ratings) 7 for either Linux or OS X, 8 if both
[**Importance:**](../project-ratings) 6

### Experience needed

Linux part will require the use of DBUS and/or DeviceKit so experience using them would be handy. OS X part obviously would be easier with some prior experience with this platform (foundation level) API.

### See also
* [Getting sleep notifications under OS X](http://developer.apple.com/library/mac/#qa/qa1340/_index.html)

