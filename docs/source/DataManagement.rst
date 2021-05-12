Cross Facility Workflows
========================
This page documents for users how to transfer data between the three ASCR Facilities.   
We also provide guidance on what storage endpoints are available across the ASCR facilities. 


Globus
-------

ALCF
~~~~~~


NERSC
~~~~~~
You can log into the Globus web interface with your NERSC credentials (by selecting NERSC in the drop down menu of supported identity providers) 
or using many of the other supported providers listed that you can authenticate against. 
NERSC maintains several Globus endpoints that can be activated for individual use by any NERSC user. 
The list of endpoints are provided in the table below. 
+----------------+---------------+------------------+
|  Endpoint Name |  Description  | Recommended Use |
+========================+============+==========+
|  NERSC DTN  |  Multi-node, high performance transfer system | Almost all data transfers needs into & out of NERSC |
|             | with access to all NERSC Global File  ||
|             | systems (NGF) as well as Cori Scratch ||
+------------------------+------------+----------+
|   NERSC HPSS          |    Single node system connected directly to the     |  Remote transfers into & out of HPSS     |
|                        |  NERSC HPSS tape archive||
+------------------------+------------+----------+
|  NERSC SHARE           |   Single node system with read-only access to      |Shared Globus endpoint|
|                         | some NERSC file systems ||
+------------------------+------------+----------+
|    NERSC S3         |    Single node system with read-only access to NERSC homes     |Data transfers to / from Amazon S3|
+------------------------+------------+----------+

* Data can be shared at NERSC using .. _Globus Sharing: https://www.globus.org/data-sharing. Currently shared endpoints are read-only, no writing is allowed. See this page for more information. 
* NERSC has an experimental Globus S3 endpoint that can be used to access and share content from AWS S3. See this page for more information. 


OLCF
~~~~~~
