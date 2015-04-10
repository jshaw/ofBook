ofBook
======

This is a collaboratively written openFrameworks book.  

**please note that this is still work-in-progress**


# Building the Book

Dependencies

- [pandoc](http://johnmacfarlane.net/pandoc/)
- [python 2.7+](https://www.python.org/)
- [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) 
- [sass](http://sass-lang.com/)
- [libsass](https://github.com/dahlia/libsass-python)
- LaTeX 
  - Windows: [MiKTeX](http://miktex.org/) is recommended 

Scripts for building the web and pdf versions of the book are in `scripts/` directory: `createWebBook.py` and `createPDFBook.py`.  You must run them from the `scripts/` directory, so either double-click the script or run it from command line.
- When building the web book, the website is stored in the `output/webBook` directory.  Opening up `output/webBook/toc.html` will open up the table of contents.
- When building the pdf book, the pdf is created at `output/ofBook.pdf`. `output/ofBook.tex` is also created, for debugging purposes.

## OSX
1. install pip at the terminal ```sudo easy_install pip```
2. install [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) (bs4) `pip install beautifulsoup4`
3. install [pandoc](https://github.com/jgm/pandoc/releases)
4. install [basictex & MacTeX-Additions](http://www.tug.org/mactex/morepackages.html)
5. install [libsass](https://github.com/dahlia/libsass-python) `sudo pip install libsass`

## Windows Installation of Dependencies
1. Download and install [Python 2.7+](https://www.python.org/)
2. Download and install [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) (bs4)
  - Method 1: 
    1. Get the python package manager, [pip](https://pip.pypa.io/en/latest/installing.html).  This involves downloading `get-pip.py` and running it from command line.
    2. Run `pip install beautifulsoup4` from the command line to install BeautifulSoup
  - Alternate [installation methods](http://www.crummy.com/software/BeautifulSoup/bs4/doc/#installing-beautiful-soup) for bs4
3. Download and install pandoc using the latest windows installer (.msi) from [here](https://github.com/jgm/pandoc/releases)
4. Download and install MiKTeX using the windows installer from [here](http://miktex.org/download)
  - When installing, check the box for "Install Packages on the Fly."  The pandoc -> PDF pipeline uses latex packages that don't all come standard with MiKTeX, so this will allow you to grab any missing packages when building the book for the first time.
5. Download and install [libsass](https://github.com/dahlia/libsass-python)
  - Using pip: `pip install libsass`

## Debian (Linux)
1. install packages: ```sudo apt-get install python-pip python2.7-dev git pandoc ruby-sass texlive```
2. install [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) and [libsass](https://github.com/dahlia/libsass-python): ```pip install beauitfulsoup4 libsass```


#Mailing List

[openFrameworks Book discussion](http://dev.openframeworks.cc/listinfo.cgi/ofbook-openframeworks.cc).

Older Book discussions can be checked at [Ofbook Archives](http://dev.openframeworks.cc/private.cgi/ofbook-openframeworks.cc/)
