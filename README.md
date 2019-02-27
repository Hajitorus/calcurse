calcurse-datefix
================

calcurse with very slightly less ill-advised date logic

calcurse maintains its data files as plain text, but uses the
least-useful date format. This tiny fork remedies that.

Note well that using this fork with an existing data file is an
Incredibly Bad idea. It does nothing to attempt to convert date formats,
and you will encounter problems if you don't convert your existing data
file before running this.

Original README.md continues below.

calcurse
========

Building
--------

Install the following build dependencies. If your distro segments development
files from core packages (i.e., \*-devel or \*-dev packages), you may need to
install those as well:

* gcc
* automake
* asciidoc
* gettext with development files
* ncurses with development files

If you are using a release tarball, the following commands can be used to build
and install calcurse:

    $ ./configure
    $ make
    $ make install

Note that `make install` needs to be run as root. When working on a Git
checkout, you need to run `./autogen.sh` before `./configure`.

Package Overview
----------------

* `build-aux`: auxiliary files for the build process
* `contrib`: useful tools such as hooks or the CalDAV synchronization script
* `doc`: detailed documentation in plain text and HTML
* `po`: translations and i18n-related files
* `scripts`: additional official scripts, such as `calcurse-upgrade`
* `src`: the actual calcurse source files
* `test`: test suite and test cases for calcurse

Authors
-------

calcurse was originally authored by Frederic Culot and is currently maintained
by Lukas Fleischer.

Of course, there are numerous other contributors. Check the Git commit log and
the `Thanks` section in the manual for a list of people who have contributed by
reporting bugs, sending fixes, or suggesting improvements.

Contributing and Donations
--------------------------

Patches, bug reports and other requests are always welcome! You can submit them
to one of our mailing lists (check the [patch submission
guidelines](doc/submitting-patches.txt) for details) or via GitHub.

We are also extremely grateful for donations which help us continue developing
calcurse as open source software and are used to cover recurring costs, such as
for our servers. You can use https://calcurse.org/donate/ for a one-time
payment. If you prefer another form of donation, do not hesitate to contact us!

Demo
----

![Demo](https://calcurse.org/images/demo.gif)
