=============
html to etree
=============

.. image:: https://img.shields.io/pypi/v/html-to-etree.svg
        :target: https://pypi.python.org/pypi/html-to-etree

.. image:: https://img.shields.io/pypi/pyversions/html-to-etree.svg
        :target: https://pypi.python.org/pypi/html-to-etree

.. image:: https://img.shields.io/travis/fluquid/html-to-etree.svg
        :target: https://travis-ci.org/fluquid/html-to-etree

.. image:: https://codecov.io/github/fluquid/html-to-etree/coverage.svg?branch=master
    :alt: Coverage Status
    :target: https://codecov.io/github/fluquid/html-to-etree

.. image:: https://requires.io/github/fluquid/html-to-etree/requirements.svg?branch=master
    :alt: Requirements Status
    :target: https://requires.io/github/fluquid/html-to-etree/requirements/?branch=master

Parse html to lxml etree

Convenience methods for parsing html documents to lxml etree.

Lxml has limited capabilities for handling different encodings, and this
library is intended as a reusable utility parsing byte-code html responses
into ElementTrees using sane character decoding.

* Free software: BSD license
* Python versions: 2.7, 3.4+

Features
--------

* Parse html to lxml etree
* Handle character decoding

Quickstart
----------

Parse HTML given as byte strings::

    tree = parse_html_bytes(body=body_bytes, content_type=res.headers.get('content-type'))

Parse HTML given as already decoded unicode string::

    tree = parse_html_unicode(uni_string=body_unicode)

Credits
-------

This package was created with Cookiecutter_ and the `fluquid/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
