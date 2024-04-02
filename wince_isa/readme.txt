Readme.txt
==========

Release 4.1  10/24/00
=====================
Release 1.0 driver was not loading in WinCE 3.0. This bug has been fixed in this release.
This bug was due to not zero-initializing the LanceChar struct, in DriverEntry, before 
filling it with the miniport entrypoints.


Release 1.0  8/20/99
=====================
The included Windows CE NDIS 4.0 Miniport driver and associated files are part
of the ISA II DMA Busmaster NDIS 4.0 Miniport driver for Windows CE. This driver has been 
compiled under the Windows CE Platform Builder Version 2.11(OEM version). 

Disk contents
=============
The source files are as follows - 

   alloc.c      -- Memory and data structure allocation modules.
   interrup.c   -- ISR, DPC(send and receive isr) modules.
   lance.c      -- Init, register, stop, start, and scan controller modules.
   request.c    -- Ndis OID set and query modules.
   send.c       -- packet send module.
   wince.c      -- installation information for the Windows CE driver / memory allocation. 
   lancehrd.h   -- Hardware related header file.
   lancesft.h   -- Software related header file.
   amddmi.h     --
   amdoids.h    --
   binsig.h     --
   lance.msg    --
   makefile     -- Makefile that called by nmake.
   makefile.inc -- 
   sources      -- build utility input file.
   pcntn4m.def  -- Export functions defined in this file. 
   pcntn4m.mc   --
   pcntn3.rc    --    

   Release.txt  -- Has build information of the driver. 


To build PCNTN4M.DLL NDIS4 miniport driver :
============================================ 
 Please refer to the Release.txt file for a detailed description of the 
build process for the CEPC platform. 

 
    

 