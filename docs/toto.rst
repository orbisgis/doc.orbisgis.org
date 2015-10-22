Toto 
========

This document will show you how to get up and running with Read the Docs.
You will have your docs imported on Read the Docs in 5 minutes,
displayed beautifully for the world.

If you are already using Sphinx or Markdown for your docs, skip ahead to
:ref:`import-docs`.

Write Your Docs
---------------

You have two options for formatting your documentation:

* :ref:`in-rst`
* :ref:`in-markdown`

.. _in-rst:

In reStructuredText
~~~~~~~~~~~~~~~~~~~

There is `a screencast`_ that will help you get started if you prefer.

Sphinx_ is a tool that makes it easy to create beautiful documentation.
Assuming you have Python_ already, `install Sphinx`_::

    $ pip install sphinx sphinx-autobuild

Create a directory inside your project to hold your docs::

    $ cd /path/to/project
    $ mkdir docs

Run ``sphinx-quickstart`` in there::

    $ cd docs
    $ sphinx-quickstart

This quick start will walk you through creating the basic configuration; in most cases, you
can just accept the defaults. When it's done, you'll have an ``index.rst``, a
``conf.py`` and some other files. Add these to revision control.

Now, edit your ``index.rst`` and add some information about your project.
Include as much detail as you like (refer to the reStructuredText_ syntax
or `this template`_ if you need help). Build them to see how they look::

    $ make html

.. note:: You can use ``sphinx-autobuild`` to auto-reload your docs. Run ``sphinx-autobuild . _build_html`` instead.

Edit your files and rebuild until you like what you see, then commit your changes and push to your public repository.
Once you have Sphinx documentation in a public repository, you can start using Read the Docs.

.. _in-markdown:

In Markdown
~~~~~~~~~~~

You can use Markdown and reStructuredText in the same Sphinx project.
We support this natively on Read the Docs, and you can do it locally::

    $ pip install recommonmark

Then in your ``conf.py``:

.. code-block:: python

    from recommonmark.parser import CommonMarkParser

    source_parsers = {
        '.md': CommonMarkParser,
    }

    source_suffix = ['.rst', '.md']

.. note:: Markdown doesn't support a lot of the features of Sphinx,
          like inline markup and directives.
          However, it works for basic prose content.

.. _import-docs:

Import Your Docs
----------------

`Sign up`_ for an account on RTD, then `log in`_. Visit your dashboard_ and click
Import_ to add your project to the site. Fill in the name and description, then
specify where your repository is located. This is normally the URL or path name
you'd use to checkout, clone, or branch your code. Some examples:
