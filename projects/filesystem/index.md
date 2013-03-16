---
layout: default
title: wxFileSystem
---

## Clean up and improve wxFileSystem

[wxFileSystem](http://docs.wxwidgets.org/trunk/classwx_file_system.html)
currently suffers from several problems, mainly confusion between the file
names and file system URIs. The goal of this project would be to clean up and
streamline the existing code to clear this up and make it possible to extend it
further.

Notably, integration with the underlying OS-specific VFS facilities such as
[GVFS](http://developer.gnome.org/gio/unstable/GVfs.html) or
[KIO](http://api.kde.org/4.2-api/kdelibs-apidocs/kio/html/index.html) might be
an interesting idea.

This proposal is not finalized, please post to wx-dev if you're interested in
discussing it further.

[**Difficulty:**](../project-ratings) ?
[**Importance:**](../project-ratings) ?

### Experience needed

Nothing particular.

### See also

