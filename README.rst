.. image:: https://img.shields.io/badge/tstn--048-lsst.io-brightgreen.svg
   :target: https://tstn-048.lsst.io
.. image:: https://github.com/lsst-tstn/tstn-048/workflows/CI/badge.svg
   :target: https://github.com/lsst-tstn/tstn-048/actions/

#####################################################################
Extending the ScriptQueue to allow parallel execution of SAL Scripts.
#####################################################################

TSTN-048
========

This technote describes a proposal to extend the ScriptQueue to execute more than one SAL Script in parallel. In its current implementation the ScriptQueue was designed to allow only one script to execute at a time. This imposes a limitation to the system when it comes to executing completely unrelated operations through the Script Queue. For example, while we take calibrations (which may take a couple hours) it is impossible to use the Script Queue to change the state of an ESS CSC. 

Here we provide an idea of extending the ScriptQueue to remove this limitation.

**Links:**

- Publication URL: https://tstn-048.lsst.io
- Alternative editions: https://tstn-048.lsst.io/v
- GitHub repository: https://github.com/lsst-tstn/tstn-048
- Build system: https://github.com/lsst-tstn/tstn-048/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally if your system has Python 3.11 or later:

.. code-block:: bash

   git clone https://github.com/lsst-tstn/tstn-048
   cd tstn-048
   make init
   make html

Repeat the ``make html`` command to rebuild the technote after making changes.
If you need to delete any intermediate files for a clean build, run ``make clean``.

The built technote is located at ``_build/html/index.html``.

Publishing changes to the web
=============================

This technote is published to https://tstn-048.lsst.io whenever you push changes to the ``main`` branch on GitHub.
When you push changes to a another branch, a preview of the technote is published to https://tstn-048.lsst.io/v.

Editing this technical note
===========================

The main content of this technote is in ``index.rst`` (a reStructuredText file).
Metadata and configuration is in the ``technote.toml`` file.
For guidance on creating content and information about specifying metadata and configuration, see the Documenteer documentation: https://documenteer.lsst.io/technotes.
