---
layout: default
title: wxRichTextCtrl-related Projects
---

## Table UI

The wxRichTextCtrl class now has text box and table capabilities, but there is
no user interface for creating and modifying tables. The goal of this project
is to analyze what's needed, looking at word processors such as OpenOffice.org
Writer, and implement the necessary dialogs and mouse manipulation (for example
table object selection and row/column movement).

----------------------------------------------------------------------------

## Right-to-left languages support

The goal is to support right-to-left languages such as Hebrew, including
support for composing individual diacritics.

### Experience needed

Good knowledge of Unicode would be helpful.

----------------------------------------------------------------------------

## Text selection

The aim would be to replace the current text selecting mechanism with a more
precise one and more correct from a visual point of view. Currently text
selection is emphasized by creating separate chunks from the selected text and
paint them separated from the rest of the text. The drawback is that often
there is a displacement of few pixels affecting the selected text compared with
the unselected text. Things are even worse if the row contains Tab characters.
As the wxRTC uses double buffering, a proposal is to have the selection
emphasized by painting the area(s) underneath the selection with the intended
color (using `wxRichTextCtrl::PaintBackground()`?), then text above it just
painted normally (maybe using a logical function with the DC). A very nice
example is in the Drawing sample in "Text screen" (F2) - the text that says
"There should be a text below".

----------------------------------------------------------------------------

## Justified text alignment

This could be done in a simpler fashion by only distributing extra space
(between words, and if needed adjust character spacing) and no hyphenation, or
more complicated by including hyphenation. The base should be a good algorithm.
Special cases: last row of a paragraph, last character in a row, images. There
is a "famous" TeX implementation but unfortunately I couldn't find any good
references for it (try [Tex (Wiki)](http://en.wikipedia.org/wiki/TeX#Hyphenation_and_justification),
[Tex (by D.Knuth)](http://tex.loria.fr/tex-source/tex-source.html)).
Another good description can be found here: Adobe InDesign, Text and
Typography. A JavaScript implementation can be found here: [TeX line breaking
algorithm in Javascript](http://www.bramstein.com/projects/typeset/). Cross
platform administrator dialog The aim would be to provide API for a
cross-platform "get administrator privileges" dialog to allow
installations/operations inside system paths. This project may include
definition &amp; implementation of an API for changing/querying access
privileges at run-time for a certain process.
