Scala workshop notes
====================

A work in progress, with pull requests gladly accepted for typos,
errata, diagrams, and other improvements.

You can simply look at these files online using github's support for
markdown. Otherwise, I've included `generate`, a simple script that
wraps `pandoc` with some standard options I use. To build a presentation
PDF:

    $ ./generate 01-workshop.md

You will need to install the dependencies for `pandoc`. 


Installing `pandoc` on Ubuntu
=============================

It's simple on Ubuntu, as might be expected:
	
    sudo apt-get install pandoc
    sudo apt-get install latex-beamer


Installing `pandoc` on OS X
===========================

For OS X, download and install the following packages:

1. pandoc DMG at https://code.google.com/p/pandoc/downloads/
2. BasicTex at http://www.tug.org/mactex/morepackages.html
3. MacTeX-Additions also at http://www.tug.org/mactex/morepackages.html


Help for generate
=================

~~~~
$ ./generate  --help
usage: generate [-h] [--format FORMAT] [--incremental] source

Simple driver for pandoc. Or use pandoc directly for more options.

positional arguments:
  source             Source markdown file

optional arguments:
  -h, --help         show this help message and exit
  --format FORMAT    Output format
  --incremental, -i  Incremental display of lists
~~~~
