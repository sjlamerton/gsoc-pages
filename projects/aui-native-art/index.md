---
layout: default
title: Native Appearance for wxAUI
---

## Implement more native art providers for wxAUI

The goal is to make wxAUI blend in better on a set of platforms, particularly
on Mac, GTK+ and Windows 7. The original wxAUI art is rather Windows XP-like
and it should be possible to take colours from the current theme and apply them
to wxAUI. Mostly this will be writing separate art provider classes, but
occasionally it may be necessary to dig deeper into the wxAUI code.

[**Difficulty:**](../project-ratings) 6
[**Importance:**](../project-ratings) 5

### Experience needed

No platform-specific experience is needed as the art provider should behave in
the same way under all platforms.

### See also

* The ribbon classes, implemented as a GSoC 2009 project, has customisable art
  and demonstrates a Vista/Windows 7-like art mode.
