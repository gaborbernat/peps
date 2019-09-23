PEP: X
Title: Persistent cache for package build
Version: $Revision$
Last-Modified: $Date$
Author: Bernat Gabor <gaborjbernat@gmail.com>
Status: Draft
Discussions-To: <distutils-sig@python.org>
Type: Standards Track
Content-Type: text/x-rst
Created: 23-Sep-2019
Python-Version: 3.9
Post-History: 12-Sep-2019


Abstract
========

This PEP adds a persistent cache directory parameter to the interface between
build frontend and build backend (as defined per PEP-517). The goal is to
allow the build frontend to control where the backend writes new files needed
to generate the resulting package. Furthermore, defines the guarantees the backend
can expect as far as reusing this cache space for improving build performance.

Rationale
=========

In PEP-517 the concept of a build backend and build frontend was introduced.

Specification
=============

Design Considerations
=====================

Implementation
==============

References
==========

.. [0] https://en.wikipedia.org/wiki/Persistent_data_structure

Acknowledgments
===============

I thank Paul Ganssle, Paul Moore and Jason R. Coombs for their feedback, ideas,
edits, and discussions around this PEP.


Copyright
=========

This document is placed in the public domain or under the
CC0-1.0-Universal license, whichever is more permissive.


..
   Local Variables:
   mode: indented-text
   indent-tabs-mode: nil
   sentence-end-double-space: t
   fill-column: 70
   coding: utf-8
   End:
