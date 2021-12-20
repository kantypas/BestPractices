APIs for Facilities
===================
This page documents programmatic interfaces to HPC resources to enable a new
paradigm of scientific endeavors, especially those that are automated or span
multiple facilities.

.. attention::

    Under construction

ALCF
~~~~
ALCF has traditionally developed the Cobalt scheduler for its systems, opening the opportunity to also expose aspects of the scheduler via a programmable API. This work is underway as part of scheduler development in preparation for the Aurora system.

NERSC
~~~~~
NERSC is developing the `SuperFacility API <https://docs-dev.nersc.gov/sfapi/>`_
that can be used to script jobs or workflows running against NERSC systems.
The goal is to support everything from a simple script that submits a job to complex
workflows that move files, check job progress and make advance compute time reservations.

Other
~~~~~
ETH's CSCS is developing `FirecREST <https://github.com/eth-cscs/firecrest>`_ to program
Petascale resource access of HPC infrastructure by using REST API