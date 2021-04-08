st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Keybindings
-----------

| Modifier | Key | Function |
--- | --- | ---
Alt | b | Send break
Control | p | Toggle printer
Shift | p | Print contents of terminal
Alt | p | Print selection
Control | plus | Increase font size
Control | minus | Decrease font size
Control | equal | Reset font size
Control+Shift | C | Copy selection to clipboard
Control+Shift | V | Paste clipboard
Control+Shift | Y | Paste selected terminal text
Shift | Page_Up | Scroll up one page
Shift | Page_Down | Scroll down one page
Alt | l | Open menu of urls in terminal, and open selected one in browser
Alt | y | Open menu of urls in terminal, and copy selected one
Alt | o | Copy output of specified command

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

