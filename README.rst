PyFrag - PSFrag, python utility
===============================

PyPfrag is a graphical tool to replace labels (tags) in EPS files into LaTeX format using PSFrag package.
Easy to use, modify and extend.

INSTALLATION
------------

It does not require installation but some python dependencies need to be fulfilled:

- gi, Gtk >= 3.10
- logging
- colorlog
- argparse
- yaml

In general, in a Debian based system is enough to run:
# apt-get install python-yaml python-colorlog

You can make an alias at ~/.bashrc
alias pyfrag='/path/to/pyfrag.py'

to be able to execute the program in a terminal.

HOW TO USE PyFrag
-----------------

PyFrag is a python script that runs in a terminal, and offers a GUI in runtime.
You need to provide the target .EPS file to the program:

$ /path/to/pyfrag.py epsfile.eps [-O options]

where /path/to/ is the directory where pyfrag.py is located.

$ pyfrag epsfile.eps [-O options]

if you have an alias established.


The program will load a default substitution file (with the script), where psfrag commands are stored.
If the file is not found it will not load any substitution.

You can provide optional substitution files with the option [-s subs-file.tex].

$ pyfrag epsfile.eps -s subs-file.tex
