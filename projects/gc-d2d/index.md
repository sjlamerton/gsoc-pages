---
layout: default
title: Direct2D-based wxGraphicsContext
---

## Implement wxGraphicsContext using Direct2D

![Drawing example](http://i.msdn.microsoft.com/ee413543.figure4%28en-us,MSDN.10%29.gif)

Currently,
[wxGraphicsContext](http://docs.wxwidgets.org/trunk/classwx_graphics_context.html)
is implemented using GDI+ under Windows. GDI+ seems, unfortunately, abandoned
by Microsoft and has a lot of problems. Generally very poor performance (as
it is not hardware-accelerated at all) and horrible text rendering, especially
at small font sizes, are just two of the most important problems.

Since Windows 7 (and Vista with updates installed) another solution is
available:
[Direct2D](http://msdn.microsoft.com/en-us/library/windows/desktop/dd370990.aspx).
This project would consist in implementing a new
[wxGraphicsContext](http://docs.wxwidgets.org/trunk/classwx_graphics_context.html)
backend using this new API, and companion DirectWrite for the text output.

[**Difficulty:**](../project-ratings) 7
[**Importance:**](../project-ratings) 8

### Experience needed

Windows, COM (at basic level), Direct2D itself would be great but can be
learned during the project.
