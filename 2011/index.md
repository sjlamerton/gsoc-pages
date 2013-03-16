---
layout: default
title: GSoC 2011
---

We had three projects during Google Summer of Code 2011:

----

### wxWidgets port for GTK+3
Student: John Chain  
Mentor: Paul Cornett

Original proposal:

> The release of GTK+3 in March and GNOME 3 in April is a big event in the
> open-source desktop community this year. Adopting GTK+3 as soon as possible
> is strategically important to the entire wxWidgets project. This GSoC 2011
> project is to port wxGTK from GTK+2 to GTK+3.

The project was a qualified success and experimental support for GTK+ 3 was
included in the next wxWidgets release.

SVN branch: http://svn.wxwidgets.org/viewvc/wx/wxWidgets/branches/SOC2011_GTK3/

----

### wxWidgets port for iOS
Student: Linas Valiukas  
Mentor: Stefan Csomor

Original proposal:

> The wxiOS project is an effort to create a wxWidgets based C++ wrapper over
> Cocoa Touch that would implement the proposed wxMobile API. The
> implementation would allow creating mobile UIs in a more generic,
> platform-independent way. If, for example, an analogue gets implemented
> for Android OS, one could expect to run the same end-user mobile
> application code on both mobile platforms without too much hassle.

This project was successful in its scope, but wxiOS still remains in highly
experimental state.

SVN branch: http://svn.wxwidgets.org/viewvc/wx/wxWidgets/branches/SOC2011_WXIOS/

----

### wxWebView Integration
Student: Steven Lamerton  
Mentor: Julian Smart

Original proposal:

> wxWidgets currently lacks any classes for modern web viewing. The built in
> wxHTML classes are only suitable for viewing simple HTML files with basic CSS
> support. This proposal aims to integrate the wxWebView patch by Marianne
> Gagnon into wxWidgets by adding build support, creating documentation and
> unit tests and finishing functionality. If time allows it also aims to add
> extra back-ends and improve the current HTML help system using the new class.

This project was spectacularly successful and
[wxWebView](http://docs.wxwidgets.org/trunk/classwx_web_view.html) was one of
the most important and highly anticipated additions in the next wxWidgets
release.

SVN branch: http://svn.wxwidgets.org/viewvc/wx/wxWidgets/branches/SOC2011_WEBVIEW/

See [previous](../2010/) and [next](../2012/) years.
