---
layout: default
title: wxWebView-related Projects
---

## Integrate and extend the Chromium backend

This project involves integrating and extending the existing wxWebViewChromium
backend for wxWebView on all platforms. Although the port current runs on
Windows and only a small amount of work should be needed for Linux support
further work is needed for Mac integration. Porting the code to the CEF3 API
would also be highly beneficial. This project has the potential to provide a
uniform backend for all three major platforms, and potentially opens the way
for better Javascript integration.

[**Difficulty:**](../project-ratings) 7
[**Importance:**](../project-ratings) 7

### See also

* [wxWebViewChromium](https://github.com/steve-lamerton/wxWebViewChromium)
* [Chromium Embedded Framework](http://code.google.com/p/chromiumembedded/)
* [wxWebView](http://docs.wxwidgets.org/trunk/classwx_web_view.html)

----------------------------------------------------------------------------

## Help system

wxWidgets currently provides the wxHtmlHelpWindow class to display HTML help
files. However it uses the wxHtmlWindow class which only supports rendering a
limited subset of the HTML standard. This project would develop a new class
wxWebHelpWindow based on wxWebView to allow complex help pages to be viewed.
This would probably involve creating a new base class wxHelpWindowBase and then
the new wxWebHelpWindow class. Other improvements could include the ability to
use the wxAuiNotebook classes rather than wxNotebook to allow a better visual
fit with classes that make extensive use of wxAUI. An EPUB parser would be a
further useful addition.

[**Difficulty:**](../project-ratings) 6
[**Importance:**](../project-ratings) 6

### See also

* [wxHtmlHelpWindow](http://docs.wxwidgets.org/trunk/classwx_html_help_window.html)
* [wxWebView](http://docs.wxwidgets.org/trunk/classwx_web_view.html)

----------------------------------------------------------------------------

## Javascript Integration

wxWebView currently provides a simple RunScript function for running
Javascript. However in many cases it would be preferable have access to a
return value, or even to call C++ from the Javascript. This project would aim
to provide at least basic functionality for accessing Javascript values. An API
would be required that ensures uniform behaviour across the different backends.
Before applying for this project please contact the wx-dev mailing list as
further research is required.

[**Difficulty:**](../project-ratings) 9
[**Importance:**](../project-ratings) 8

### See also

* [wxWebView](http://docs.wxwidgets.org/trunk/classwx_web_view.html)

----------------------------------------------------------------------------

## General Improvements

Although a solid base was created as a Summer of Code 2011 project there is
still much work that can be done to improve wxWebView and its associated
classes. Recommended areas to work on include ways to manage scripts (enabling
and disabling javascript etc) and plugins (enabling and disabling plugins e.g.
flash / java). Other areas of potential work include improving printing support
and support for proxies and authentication. It is expected that a number of
these areas would be improved as part of a project, ideally on all three
existing backends, whilst also keeping the new Chromium backend in mind. Please
post to wx-dev if you are interested in working on this so that work is not
duplicated.

[**Difficulty:**](../project-ratings) 7
[**Importance:**](../project-ratings) 6

### See also

* [wxWebView](http://docs.wxwidgets.org/trunk/classwx_web_view.html)
