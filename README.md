# High Performance Computing (HPC) Cluster modernization

## Specifications

### Description of project

Wright State University would like to modernize its current High Performance Computing (HPC) Cluster to support research and education programs. The HPC cluster is utilized by researchers from a number of disciplines and this modernization will allow faculty to make use of the latest networking, processing, and storage technologies in our current HPC environment.

### Summary of HPC cluster

The current cluster has 24 identical compute nodes, 1 Graphics Processing Unit (GPU) node with 8x NVIDIA Tesla P100 GPU cards, and 1 login node. The proposed modernization will add high speed networking to all existing nodes for data transfer speeds approaching 100Gb/s. All additional hardware must also connect to this new high speed network. The preferred network cards for this upgrade will support PCIe 3.0x16. In addition to the 26 network cards, a 48 port switch and all needed cables will be included.

To support more GPU computational tasks, we will be splitting the GPU's out of our 8x NVIDIA Tesla compute node into a new server. This server should have 2x Intel Xeon Gold 6330 or equivalent processors, 256GB RAM, and room for 4 NVIDIA Tesla P100 GPU cards (to be taken from existing server). In addition to this, two new GPU nodes are needed with the same specifications as the empty accelerator node and a NVIDIA A100 Tensor Core GPU.

The final upgrade to the HPC cluster will be a central storage system to facilitate shared storage on all compute nodes (CPU and GPU). This storage should operate independently from all compute nodes and be accessible by all compute nodes (and login nodes) via the 100Gb/s network. Disk I/O speeds should be able to support HPC workloads running on multiple compute nodes simultaneously. Storage capacity should be over 50TB usable capacity. All relevant meta data or other servers required for this storage should be included in the quote and clearly stated they are needed for the storage system to operate.

### Hardware Specification

#### **Login Node (1x)**

Login node should at least have:

* (2x) Intel 28-Core Xeon Gold 6330
* 256GB DDR4 3200MHz RAM
* (2x) 480GB M.2 SSD
* (2x) 10Gb RJ45 networking
* (1x) PCIe 3.0x16 network card supporting 100Gb/s
* Redundant 1300W PSU
* IPMI/iKVM with dedicated 1Gb RJ45
* Relevant power and networking cables
* Half extension rails for rack mount
* 3 year standard warranty

#### **Empty GPU accelerator node**

0 GPU accelerator node should at least have:

* (2x) Intel 28-Core Xeon Gold 6330
* 256GB DDR4 3200MHz RAM
* (2x) 480GB M.2 SSD
* (2x) 10Gb RJ45 networking
* (1x) PCIe 3.0x16 network card supporting 100Gb/s
* (4x) empty PCIe 3.0x16 slots for GPUs
* (3x) Redundant 1600W PSU
* IPMI/iKVM with dedicated 1Gb RJ45
* Relevant power and networking cables
* Half extension rails for rack mount
* 3 year standard warranty

#### **(2x) Single GPU accelerator node**

Each of the 2 GPU accelerator nodes should at least have:

* (2x) Intel 28-Core Xeon Gold 6330
* 256GB DDR4 3200MHz RAM
* (2x) 480GB M.2 SSD
* (2x) 10Gb RJ45 networking
* (1x) PCIe 3.0x16 network card supporting 100Gb/s
* (4x) empty PCIe 3.0x16 slots for GPUs
* (3x) Redundant 1600W PSU
* (1x) NVIDIA A100 Tensor Core GPU
* IPMI/iKVM with dedicated 1Gb RJ45
* Relevant power and networking cables
* Half extension rails for rack mount
* 3 year standard warranty

#### **Storage system**

Storage system should at least have:

* (2x) Intel 28-Core Xeon Gold 6330
* 256GB DDR4 3200MHz RAM
* (3x) RAID controllers (cache/backup protection)
* (24x) 2.5" sata/SAS drive bays
* (2x) 480GB M.2 SSD
* (24x) 4TB SSD
* (2x) 10Gb RJ45 networking
* (1x) PCIe 3.0x16 network card supporting 100Gb/s
* Redundant 1300W PSU
* IPMI/iKVM with dedicated 1Gb RJ45
* Relevant power and networking cables
* Half extension rails for rack mount
* 3 year standard warranty

#### **Networking**

In addition to any above system networking, to upgrade our current cluster to the new 100Gb/s network the following are needed:

* (1x) 48 port 100Gb/s network switch
* (26x) 100Gb/s network card, PCIe 2.0 x16
* (32x) 3 meter network cable
* 3 year standard warranty an all network equipment

#### **Additional equipment for expansion**

It is the responsibility of the vendor to contact Wright State University to ensure all needed equipment to install and operate this HPC modernization is included. This may include Power Distribution Units (PDUs), additional network cables and switches, blank panels, iKVM consoles, etc.

#### **Cluster assembly and configuration

* The HPC cluster and additional networking equipment must be assembled by the vendor on-site. Installation will include moving the components into Wright State University data-centers, connecting to data-center power and networking, system updating and driver installation, system verification and orientation, and trash removal.

#### **Software**

* Latest RedHat Enterprise Linus Operating System (perpetual license if applicable) with latest updates for all existing and new nodes.
* Setup and configured common file-system will allow all compute nodes access to the same files and write to both the common file-system and local scratch storage.
* A HPC cluster management/monitoring solution compatible with all equipment is required.
* Singularity container software
* Slurm job scheduling software
* It licensed software is installed the the software licenses should be provided for at least 3 years (prefer 5 years)
* Vendor must coordinate software list with Wright State University representative to finalize installation

#### **Warranty**

**Please state warranty terms clearly.**

* Provide a 3 year upfront warranty with a minimum level or 8x5 next business day email, phone, and online support. Must also provide advance replacement coverage for exchange of malfunctioning parts. Also provide a quote for hardware support for the 4th and 5th year of warranty at the same level.
* Provide the life cycle of the hardware. It is preferred that the equipment purchased from the vendor includes lifetime technical support.
* Warranty and support must be provided by the equipment manufacturer, not a 3rd party.

#### **Documentation**

Must provide detailed documentation of cluster hardware configuration, including old and new nodes, compute node configuration, hardware component replacement instructions, and software user manuals (if applicable).


