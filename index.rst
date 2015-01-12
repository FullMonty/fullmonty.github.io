.. The Full Monty documentation master file, created by
   sphinx-quickstart on Mon Jan 12 21:41:56 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

###################################################
The Full Monty scientific Python installers for OSX
###################################################

The Full Monty installers give you the whole `scientific Python stack <scipy
stack_>`_ in one easy-to-swallow installer package for OSX.

We recommend you use these installers with Python from the `Python.org`_
installers.  First install Python.org Python, then download and install from
the disk images here.

You can also use these disk images to install on homebrew_ and macports_ using
the command line |--| see the README file on the disk images for instructions.

Please don't use the Python that comes with OSX, it will cause you `no end of
problems <which python_>`_ with scientific Python packages.

*********
Downloads
*********

* `Full Monty disk image for Python 2.7 <https://3f23b170c54c2533c070-1c8a9b3114517dc5fe17b7c3f8c63a43.ssl.cf2.rackcdn.com/scipy-stack-py27-1.1.dmg>`_
* `Full Monty disk image for Python 3.3 <https://3f23b170c54c2533c070-1c8a9b3114517dc5fe17b7c3f8c63a43.ssl.cf2.rackcdn.com/scipy-stack-py33-1.1.dmg>`_
* `Full Monty disk image for Python 3.4 <https://3f23b170c54c2533c070-1c8a9b3114517dc5fe17b7c3f8c63a43.ssl.cf2.rackcdn.com/scipy-stack-py34-1.1.dmg>`_

*********************************************
Why would I use your installer instead of ...
*********************************************

Other free OSX installer bundles that you might consider are:

* `Anaconda`_ : maintained and supported by `Continuum analytics`_ and using
  an alternative component package installer and binary format called
  `conda`_.
* `Enthought Canopy`_ : maintained and supported by `Enthought`_.
* `Scipy SuperPack`_ : a script for building the Python scientific stack on
  OSX. Scipy superpack uses homebrew_ and pip_ to build and install a similar
  set of Python libraries.

As for Anaconda and Canopy, you'll like the Full Monty installer if you want a
double-click installer that will install the standard scientific Python
packages in one go.  Like Anaconda and Canopy, you do not need a compiler for
the install, although you probably will want to install the `Xcode command
line tools`_ at some point in your scientific Python career.

If you are already using the standard Python.org Python, then the Full Monty
might be a good option, because it installs into the Python.org Python
directories, rather than the Anaconda and Canopy approach of installing into
an alternative build of Python.  If you are using homebrew_ or macports_, you
might like the fact that you can use the Full Monty disk image as a source of
packages to install into homebrew or macports Python.

Anaconda and Canopy contain many more packages than just the scientific Python
stack, so if you want to install large packages like PyQt_ or VTK_ then you
will probably prefer something like Anaconda or Canopy.

You might or might not like the fact that the Full Monty is entirely supported
with volunteer effort and has no ties to a company.  It is built from the
public binary packages available from the `Python Package index <pypi_>`_.

*****************
How does it work?
*****************

The Full Monty installer uses the `pip`_ tool to do the all the work of
installing the component Python packages.  Pip is the standard package
installer for Python, `recommended <pypa recommended_>`_ by the `Python
packaging authority`_.  The Full Monty will install pip for you, if you don't
have it, and upgrade pip to the latest version if you do.

You can always do something very similar to the Full Monty installer using the
pip command line, but the installer means you can download a single disk image
file that contains a set of packages that are known to work together.

How do we know they work together?  Because we test them automatically using
the `Travis public testing service <travis-ci_>`_ - see `wheels2dmg on
travis-ci`_.

Anyone is welcome to come help maintain these installers.  We build them with
the `wheels2dmg`_ package, available on Github, and use the standard `Python
Packaging Authority`_ wheels_ binary package format for the component
packages.

*****************************
What packages do you install?
*****************************

The list of packages comes from the `wheels2dmg travis configuration`_:

The packages are:

* pip_;
* numpy_;
* scipy_;
* matplotlib_;
* `ipython`_ (including the IPython notebook);
* pandas_;
* numexpr_;
* sympy_.

If you need anything else, you can usually install it with pip.  Say you want
the `scikit-learn`_ machine learning package.  First run the Full Monty
installer, then open Terminal.app and run::

    pip install scikit-learn

**********
Installing
**********

It is the usual OSX install routine:

* Download the disk image for the Python that you are using;
* Double click on the disk image to mount it;
* Right click and select open to open the ``.pkg`` installer file on the disk
  image;
* Say yes to install a mountain of scientific Python quality.

*******
Support
*******

Please drop us a line on the `wheels2dmg issue tracker`_ and we'll do our best
to help.

.. include:: links_names.inc
