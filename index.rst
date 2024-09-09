#####################################################################
Extending the ScriptQueue to allow parallel execution of SAL Scripts.
#####################################################################

.. abstract::

   This technote describes a proposal to extend the ScriptQueue to execute more than one SAL Script in parallel. In its current implementation the ScriptQueue was designed to allow only one script to execute at a time. This imposes a limitation to the system when it comes to executing completely unrelated operations through the Script Queue. For example, while we take calibrations (which may take a couple hours) it is impossible to use the Script Queue to change the state of an ESS CSC. 

Here we provide an idea of extending the ScriptQueue to remove this limitation.

Add content here
================

See the `Documenteer documentation <https://documenteer.lsst.io/technotes/index.html>`_ for tips on how to write and configure your new technote.
