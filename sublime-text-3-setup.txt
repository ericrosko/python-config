Sublime text, install package control:
google “sublime text package control”, click install, copy the text command, go View→Show Console, paste the text in and hit Enter.

cmdl+shift+p opens up the package control textbox
- Now type “Install”, hit Enter.
- Now you will get to type to autocomplete from packages it finds.
- install Daylee color schemes.  just type “Daylee” and it should appear.
I see now in my Installed Packages folder I have: Dayle Rees Color Schemes.sublime-package

Packages:
BracketHighlighter - shows matching brackets
To uninstall a package, type ‘remove package’ or similar, then Enter, then type name of package to remove.
SidebarEnhancements - lots of new options when right clicking in the sidebar
SublimeCodeIntel - intellisense for everything.


    For Mac OS X:
      * Jump to definition = ``Control+Click``
      * Jump to definition = ``Control+Command+Alt+Up``
      * Go back = ``Control+Command+Alt+Left``
      * Manual CodeIntel = ``Control+Shift+space``

    For Linux:
      * Jump to definition = ``Super+Click``
      * Jump to definition = ``Control+Super+Alt+Up``
      * Go back = ``Control+Super+Alt+Left``
      * Manual CodeIntel = ``Control+Shift+space``

    For Windows:
      * Jump to definition = ``Alt+Click``
      * Jump to definition = ``Control+Windows+Alt+Up``
      * Go back = ``Control+Windows+Alt+Left``
      * Manual CodeIntel = ``Control+Shift+space``

SublimeLinter  (do not install SublimeLint which is different)
  you then must install a package for each langauge you want to support.
  you also need Node.js installed.
  you must google SubmlimeLinter JSLint (or CSSLint), then do the command line they say, and only then can you got cmd+shift+p and install the specific linter in Sublime Text. ie SublimeLinter-CssLint, or SublimeLinter-(you language here)

*********

http://cheng.logdown.com/posts/2015/06/14/sublime3-install-python-linters

Sublime3 install python linters
Linters are used to highlight syntax and style errors in your source code. It is very useful to have when writing python, js, css, YAML, etc.

To enable linting in Sublime text 3, a few things need to be installed to get it working.

1) Install Sublime Linter first. This is a framework rather than an actual linter that can inspect your code. When we install other linters, they will depend on this framework. Thus, it is important to install this 'mother base' first.

  - open up package control, cmd+shift+p on Mac OS X, ctrl+shift+p on Linux/Windows
  - type 'install' and select 'Package Control: Install Packages'
  - type 'SublimeLinter'
2) Install pep8 and pyflake. These python libraries will be used by the linters installed in the next step. Open up a console window, and install them by:

pip3 install pep8 pyflakes
The pep8 package is for style checking and pyflakes is for syntax error checking.

NOTE: make sure you are not installing these packages while using virtualenv. This is the mistake that I made. These pacakges need to be available system wide.

3) Install the actual linters: Sublime Linter-pyflakes, Sublime Linter-pep8:

open up package control, cmd+shift+p on Mac OS X, ctrl+shift+p on Linux/Windows
type 'install' and select 'Package Control: Install Packages'
type 'pep8' and find 'SublimeLinter-pep8'
type 'pyflakes' and find 'SublimeLinter-pyflakes'
4) After everything has been installed, restart sublime text 3

5) Now you should see error highlights in the gutter and around the code. To set when linting should be active, right click anywhere in Sublime Text 3 and select 'SublimeLinter' > 'Lint Mode'

6) It is very likely that pep8 will point out a few styling errors. It is anonying to fix them by hand. We can use another plugin to autoformat python code for us. Install Python PEP8 Autoformat via package control.

After this is installed, press 'ctrl + shift + r' to perform auto format.

7) pep8 linter is likely to complain about using 4 spaces instead of tabs when writing Python code. You can change this in Sublime's setting File. Go to 'Sublime Text > Preferences > Settings - User', add the following lines:

after installing pep8 autoformat, do this:
After this is installed, just open a file and 'ctrl + shift + r' to perform auto format.  The file is auto formatted!

cmd+k+cmd+b to show/hide sidebar
