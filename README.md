# rwbatools
Tools for teaching Python

Key tool right now is gui

This provides a library for implementing easy GUIs...

Download the package, unzip it, make sure the folder is called rwbatools

Add rwbatools to your PYTHONPATH (export PYTHONPATH=$PYTHONPATH:~/Downloads/rwbatools)

And give it a twirl.
 - Check the docs folder, for a couple of PDFs with help.
 - Check the Lessons folder, for some example code.

Example:

  from rwbatools import gui
  app = gui("Example")
  app.addLabel("label1", "Hello World")
  app.go()

Reasoning:
 - Designed to be as easy as possible, yet still provide a lot of tkinter functionality
 - Provides 3 functions for most widgets:
   - add(name, value) this adds a new widget (usually with a name and a value)
   - set(name, value) this updates the value of the named widget
   - get(name) this gets the value of the named widget
 - Uses grid layout
 - When adding widgets, up to 3 numerical "positions" can be supplied:
   - column - the coloumn to appear in, starting at 0
   - row - row to appear in, stating at 0
   - span - how many columns to span across
 - Provides loads of extra bits and pieces outside of core tkinter
   - Some of this was from the excellent resources @ http://effbot.org
   - Some of this was from slashdot examples of how to solve common problems
   - Some of this has been incorporated from other people's modeules:
     - Michael Lange's ToolTip
     - Johann C. Rocholl's tkinter_png support
     - Martin J. Fiedler's NanoKPEG library
 - I've tried to get as much functionality into this library as possible, without requireing any other modules

Caveats.
 - Although an experienced developer, I knew nothing of Python when I started this
 - Built for Python3
 - Built under a Windows environment (at school)
 - Tested (somewhat) on Mac OSX (at home)
 - There are no promises here, it grew quite quickly, and hasn't had enough testing
 - If you find problems, let me know and I'll fix them
 - There are limitations...