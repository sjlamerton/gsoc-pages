---
layout: default
title: Improving wxUniversal
---

## Fix bugs and implement missing features in wxUniversal

[wxUniversal](http://www.wxwidgets.org/about/wxuniv.htm) is a special
wxWidgets port which implements high-level GUI controls using wxWidgets itself
instead of wrapping the native toolkit as all the other ports do. It is useful
for platforms which don't have their own native UI (such as e.g.
[DirectFB](http://directfb.org/)) or those in which the native UI is difficult
to wrap (see the discussion of [wxAndroid](../project/android) project).

Unfortunately wxUniversal hasn't got much attention for many years and the
changes elsewhere in wxWidgets have introduced quite a few bugs in it. Also
many relatively recent controls are not implemented.

The goal of this project would be to check the current wxUniv status in
detail, catalog the existing bugs and missing features and, based on this
list, work on fixing and implementing them.

[**Difficulty:**](../project-ratings) 7
[**Importance:**](../project-ratings) 6 (but more if wxUniv is used by wxAndroid)

### Experience needed

Some prior experience with wxWidgets would be helpful, as with any other
project, but no platform/toolkit-specific knowledge is needed for this task.

### See also

* [Incomplete list of wxUniv bugs](http://trac.wxwidgets.org/query?status=accepted&status=confirmed&status=infoneeded&status=infoneeded_new&status=new&status=portneeded&status=reopened&component=wxUniv+%28any+port%29&order=priority&col=id&col=summary&col=status&col=type&col=priority&col=milestone&col=component)
