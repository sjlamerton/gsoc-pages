---
layout: default
title: System sounds
---

## Cross platform support for playing system sounds

wxWidgets provides a wxBell() function which is as simple as it gets and the wxSound
class which allows sound files to be played but requires the file (or sound data)
to be present and produces the same result under all platforms (meaning that it
won't sound good on any of them). The goal of this project would be to
provide a way to play various "system sounds" in a simple and portable way and
respecting the user settings (in particular, not play anything at all if the
sound effects are turned off).

[**Difficulty:**](../project-ratings) 5-7
[**Importance:**](../project-ratings) 5

Difficulty is 5 is for a minimal usable implementation, 7 for something
sufficiently powerful to represent libcanberra API while still being
implementable on the other platforms.

### See also

* [Windows example](http://www.codeproject.com/Articles/2740/Play-Windows-sound-events-defined-in-system-Contro) (not sure if this is the best way though)
* [OS X system sound reference](http://developer.apple.com/library/mac/#documentation/AudioToolbox/Reference/SystemSoundServicesReference/Reference/reference.html)
* [libcanberra](http://developer.gnome.org/libcanberra/) from Freedesktop, i.e. modern Linux systems.


### Experience needed

Experience with the platforms being targeted would be welcome.
