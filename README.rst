=============================
Olimpiada Matemática del D.F.
=============================

Get started by cloning this repository

.. code:: sh

   $ git clone https://github.com/imatem/omdf-buildout.git

First, copy the ``buildout.cfg_tmpl`` into the buildout root. The
``profiles/testing.cfg`` profile is active by default, but you can use any of
the others. See descriptions below.

.. code:: sh

    $ cd omdf-buildout
    $ cp profiles/buildout.cfg.tmpl buildout.cfg

Then you need to run::

 $ virtualenv env

This will create an env directory with a virtual environment. You should then
install the versions of ``zc.buildout`` and ``setuptools`` you need

.. code:: sh

   $ env/bin/pip install -r requirements.txt

To create an instance, run

.. code:: sh

   $ env/bin/buildout

This will download Plone's eggs and products for you, as well as other
dependencies, create a new Zope 2 installation, and create a new Zope instance
configured with these products.

You can start your Zope instance by running

.. code:: sh

   $ bin/instance fg
