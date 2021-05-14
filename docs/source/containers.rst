Containers
==========
This page documents container infrastructure available at each site.

.. attention::

    Under construction

ALCF
~~~~

NERSC
~~~~~

.. image:: https://www.nersc.gov/assets/_resampled/ResizedImageWzYwMCw0NTNd/shifterDiagram.png

`Shifter <https://www.nersc.gov/research-and-development/user-defined-images/>`_
is a software package that allows user-created images to run at NERSC.
These images can be `Docker images <https://docs.docker.com/engine/reference/commandline/images/>`_ or other formats.
Using Shifter you can create an image with your desired operating system and easily 
install your software stacks and dependencies. 
If you make your image in Docker, it can also be run at any other computing center that is Docker friendly. 
Shifter also comes with improvements in performance, especially for shared libraries. 
It is currently the best performing option for python code stacks across multiple nodes. 
For full information on using Shifter at NERSC, please see `this page <https://docs.nersc.gov/development/shifter/how-to-use/>`_.

OLCF 
~~~~
