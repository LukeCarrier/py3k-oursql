oursql v0.9.3 (for Python 3)!
=============================

About this fork
---------------

Having being totally unable to find any sort of authority in terms of the
development and maintenance of this module, and having run into issues with
distribute (the package in PyPI seems to be broken for some completely unknown
reason) and a minor bug in oursql.c, I've decided to repackage this module on
github with a couple of minor fixes:

* you can generate an egg by cd'ing into the source directory and executing
  python3.3 setup.py bdist_egg
* cursors no longer throw these errors:
  '_DictStatement' object has no attribute 'charset'

The usual warning
-----------------

I screw up sometimes. My knowledge of Python's internals is incredibly
limited. If this breaks things (no matter how unlikely), I apologise, but I
cannot be held liable for any damage caused.

Installing
----------

The installation process is pretty simple:

* Install distribute (use 0.6.19, or visit
  [this bug ticket](https://bitbucket.org/tarek/distribute/issue/206) to fix
  the errors about httplib)
* Install cpython via easy_install:
  easy_install-3.3 cpython
* Clone the repository:
  git clone git@github.com:LukeCarrier/py3k-oursql.git
* Build the module:
  cd py3k-oursql
  python3.3 setup.py bdist_egg
* Install said module:
  easy_install-3.3 dist/*.egg

More information
----------------

Comprehensive documentation for oursql is available online:
http://packages.python.org/oursql/
