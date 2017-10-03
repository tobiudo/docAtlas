*****
ATLAS
*****

Salchicha
#########

Getting started
###############

Log into the system
*******************

1. Log in to the access node ac.sw.ehu.es:
::
 ssh username@ac.sw.ehu.eus
   
You can also establish connection with login nodes manually:
::
 ssh username@ac-01.sw.ehu.eus
 ssh username@ac-02.sw.ehu.eus
   
2. Establish connection with atlas.sw.ehu.es:
::
 ssh username@atlas.sw.ehu.eus
 
You would need to bring your files and data over, compile your code or use the compiled one, and create a batch submission script. Then submit that script so that your application runs on the compute nodes. Pay attention to the various file systems available and the choices in programming environments.

SSH key generation
==================

Technical details
*****************

Atlas nodes run CentOS 7.2 and are managed with batch services through Torque 4.2.10 and Maui 3.3.1. Global scratch storage area is supported by a BeeGFS parallel distributed file system with 6 I/O servers. Inter-node communicationis through a FDR InfiniBand network.

Compute nodes are housed in 4 racks. Each node has two Intel Xeon E5-2680 v3/E5-2683 v4. Nodes are configured with 128GB/256Gb/512GB memory.

.. figure:: atlas.png
   :scale: 100 %
   :alt: Atlas cluster during maintenance
   :align: center
	   
The interconnect is an FDR InfiniBand network of Mellanox switches, consisting of a ring topology over 5 switches.

The configuration and features for the compute nodes, interconnect and I/O systems are described below.

+--------------------------------------------------------------------------------------------------+
|                                           Specifications                                         |
+===================+==============================================================================+
| **Purchase year** | 2015, 2016, 2017                                                             |
+-------------------+------------------------------------------------------------------------------+
|     **Nodes**     | 17 nodes with 2 12-core Intel Xeon E5-2680 v3 at 2.50GHz and 500GB of RAM.   |
+-------------------+------------------------------------------------------------------------------+
|    **Network**    |                                                                              |
+-------------------+------------------------------------------------------------------------------+


Running jobs on Atlas
#####################

Submitting your jobs
********************


Monitoring and managing jobs
****************************

Accounting
**********

Batch script examples
*********************


File storage and I/O
####################


Software
########

For a more detailed explanation about how to use installed software on Atlas, please refer to <Environment Modules> section.

How to look for specific software
*********************************

Applications
************

Compilers
*********

Libraries
*********

Profiling and debugging tools
*****************************


Limits
######

.. math::
   :nowrap:
      
      \begin{eqnarray}
      y    & = & ax^2 + bx + c \\
      f(x) & = & x^2 + 2xy + y^2
      \end{eqnarray}
      
Soft limits
***********
      
Hard limits
***********
