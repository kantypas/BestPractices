Data Management
========================
This page documents for users how to transfer data between the three ASCR Facilities.   
We also provide guidance on what storage endpoints are available across the ASCR facilities. 


.. attention::

    Under construction

Globus
-------

ALCF
~~~~~~
https://www.alcf.anl.gov/support-center/theta/using-globus-theta

https://www.alcf.anl.gov/support-center/cooley/globus-cooley


NERSC
~~~~~~
You can log into the Globus web interface with your NERSC credentials (by selecting NERSC in the drop down menu of supported identity providers) 
or using many of the other supported providers listed that you can authenticate against. 
NERSC maintains several Globus endpoints that can be activated for individual use by any NERSC user. 
The list of endpoints are provided in the table below. 


+----------------+-----------------------------------------------+---------------------------+
|  Endpoint Name |               Description                     | Recommended Use           |
+================+===============================================+===========================+
|  NERSC DTN     | Multi-node, high performance transfer system  | Almost all data transfers |
|                | with access to all NERSC Global File          | needs into & out of NERSC |
|                | systems (NGF) as well as Cori Scratch         |                           |
+----------------+-----------------------------------------------+---------------------------+
|   NERSC HPSS   | Single node system connected directly to      | Remote transfers into &   |
|                | the NERSC HPSS tape archive                   | out of HPSS               |
+----------------+-----------------------------------------------+---------------------------+
|  NERSC SHARE   | Single node system with read-only access to   | Shared Globus endpoint    |
|                | some NERSC file systems                       |                           |
+----------------+-----------------------------------------------+---------------------------+
|    NERSC S3    | Single node system with read-only             | Data transfers to  & from |
|                | access to NERSC homes                         | Amazon S3                 |                   
+----------------+-----------------------------------------------+---------------------------+


* Data can be shared at NERSC using `Globus Sharing <https://www.globus.org/data-sharing>`_. Currently shared endpoints are read-only, no writing is allowed. See `this page <https://docs.nersc.gov/services/globus/#sharing-data-with-globus>`_ for more information. 
* NERSC has an experimental Globus S3 endpoint that can be used to access and share content from AWS S3. See `this page <https://docs.nersc.gov/services/globus/#globus-s3-endpoint>`_ for more information. 



OLCF
~~~~~~

OLCF uses Globus for large bulk transfers into and out of the facility. 
Documentation is available for `transfers from personal computing devices <https://docs.olcf.ornl.gov/data/transferring.html#using-globus-from-your-local-machine>`_ as well as endpoints from one facility to another. 
See `this page <https://docs.olcf.ornl.gov/data/transferring.html>`_ for more information. 

The recommendation to transfer files in and out of OLCF is to begin from the external site, and tar files before executing a transfer between endpoints.


+----------------+-----------------------------------------------+---------------------------+
|  Endpoint Name |               Description                     | Recommended Use           |
+================+===============================================+===========================+
|  OLCF DTN      | Multi-node, high performance transfer system  | Almost all data transfers |
|                | with access to OLCF centewide file system     | needs into & out of OLCF  |
+----------------+-----------------------------------------------+---------------------------+
|   OLCF HPSS    | Single node system connected directly to      | Remote transfers into &   |
|                | the NERSC HPSS tape archive                   | out of HPSS               |
+----------------+-----------------------------------------------+---------------------------+



DataFed
---------

DataFed is a federated and scalable scientific data management and collaboration system that addresses the critical need for holistic 
and FAIR-principled “big data” handling within, and across, scientific domains and facilities with the goal of enhancing the 
productivity and reproducibility of data-oriented scientific research. 
DataFed supports the early lifecycle stages of “working” scientific data and serves as a tool to ease the burden associated with capturing, 
organizing, and sharing potentially large volumes of heterogeneous scientific data. 
DataFed provides an environment in which scientific data can be precisely controlled and refined in preparation for eventual data publishing.

See `this page <https://ornl.github.io/DataFed/>`_ for more detailed documentation. 


