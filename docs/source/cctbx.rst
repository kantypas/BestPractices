Using CCTBX in a Superfacility Workflow
=======================================

Realtime data analysis is a powerful tool, enabling rapid descision making
during experiments. Unlike traditional simulation workloads, fast feedback, and
automatic data management are central features of this workflow. We therefore
use a "Superfacility" paradigm to computing, where HPC is a reactive element
which is tightly coupled to the experiment's data processing pipeline. `A
recent publication <https://arxiv.org/abs/2106.11469>`_ demonstrates these
workflows at NERSC. Critical for resiliancy is to enable failover to other
facilities.

The following figure outlines the LCLS + NERSC workflow. We improved
portability by employing the following technologies:

1. Enable data to be "sent everywhere" at short notice.
2. Build protable containers for the data analysis software. This allows rapdi
   re-deployment at a new site.
3. Host workflow orchestration on Kubernetes-based microservices platforms.
   This minimizes the amount of custom (site-local) pipeline management code.

.. figure:: ./assets/cctbx_workflow.png

   Example of the NERSC-LCLS Superfacility workflow. Data is collected at LCLS
   (upper left box) where it is stored on disk. Once an experimental run is
   completed, a XRootD cluster automatically copies all of the files for that
   run to the SCRATCH Lustre file system at NERSC (central arrow -- orange
   spikes show instantaneous data transfer rate over ESNet, each spike being
   the data for one run). Once the data for a run has been completely
   transferred to NERSC, the cctbx.xfel pipeline management tool (running on a
   login node, bottom left box) automatically submits data analysis jobs
   (running in shifter containers, bottom right box). The data analysis at
   NERSC are coordinated by a MySQL database hosted on the Spin microservices
   platform (bottom center box).


CCTBX
-----

The Crystallographic Toolbox (CCTBX)


Portability
-----------
