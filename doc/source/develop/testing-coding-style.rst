`Home <index.html>`_ SaltStack-Formulas Development Documentation

====================
Testing Coding Style
====================

.. contents::
    :backlinks: none
    :local:

Formulas are pre-written Salt States. They are as open-ended as Salt States
themselves and can be used for tasks such as installing a package,
configuring, and starting a service, setting up users or permissions, and many
other common tasks. They have certain rules that needs to be adhered.


Using Double Quotes with no Variables
=====================================

In general - it's a bad idea. All the strings which does not contain dynamic
content ( variables ) should use single quote instead of double.


Line Length Above 80 Characters
===============================

As a 'standard code width limit' and for historical reasons - [IBM punch
card](http://en.wikipedia.org/wiki/Punched_card) had exactly 80 columns.


Single Line Declarations
========================

Avoid extending your code by adding single-line declarations. It makes your
code much cleaner and easier to parse / grep while searching for those
declarations.


No Newline at the End of the File
=================================

Each line should be terminated in a newline character, including the last one.
Some programs have problems processing the last line of a file if it isn't
newline terminated. [Stackoverflow
thread](http://stackoverflow.com/questions/729692/why-should-files-end-
with-a-newline)


Trailing Whitespace Characters
==============================

Trailing whitespaces take more spaces than necessary, any regexp based
searches won't return lines as a result due to trailing whitespace(s).


--------------

.. include:: navigation.txt
