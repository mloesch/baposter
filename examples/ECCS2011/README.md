Revision info
=============
* $LastChangedDate: 2011-09-11 10:59:34 +0200 (V, 11 szept. 2011) $
* $LastChangedRevision: 129 $
* $LastChangedBy: rlegendi $
* $Id: README.md 129 2011-09-11 08:59:34Z rlegendi $

General Notes
=============
The poster was created with the help of Brian Amberg's [LaTeX Poster Template][].

The source is a bit commented, however, there are some minor caveats one should be aware of when compiling them.

Compiling the sources
=====================
I ran into some minor issues while using the template. Ain't sure ir it is an issue on other systems (I had Windows 7x64 with MiKTeX v2.8).

**The best way to evade them is to use pdflatex instead of latex to create the poster.** If it is required, `latex` may also be used, you can find some minor workarounds for the issues rising below.

No background image is displayed
--------------------------------
Clean the project by deleting the following files:

- `poster.aux`
- `poster.dvi`
- `poster.log`

Then recompile the sources. The background image should be displayed.

Backround image positioning problem workaround
--------------------------------------------------
1. First, change the document class options as follows:

		%\documentclass[a0paper,portrait]{baposter}
		\documentclass[a4paper,portrait]{baposter}

  Just change `a0paper` to anything else (`a4paper` just worked for me, ain't sure about the others).
2. Compile the sources.
3. Change back the document class definition to `a0paper`, and the result should show the background image properly.



[LaTeX Poster Template]: http://www.brian-amberg.de/uni/poster/
                         "Brian's Template"

