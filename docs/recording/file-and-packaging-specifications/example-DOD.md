---
layout: default
title: Example DOD Package
parent: File and Packaging Specifications
grand_parent: Recording
nav_order: 2
---

## Example DOD Package Specifications
The document outlines file and packaging specifications for recording for Dance Original Documentation (DOD). If you have questions about the specifications please contact [Digital Preservation](mailto:digitalarchives@nypl.org) staff for guidance.

## File Classes

* Archive Original (AO): **Required**
* Edit Masters (EM): **Required**
* Service Copies (SC): **Required for both Archive Originals and Edit Masters** 
* Images: N/A
* Project Files: N/A
* Captions: If requested by Curator. 
* Transcripts: N/A

## Example with only required elements

(to be reworded)
The following is an example file structure of a performance recorded with a Sony camera capturing to XAVC and a GoPro capturing to its native format. This file structure uses just required file classes. 

```
ncov421
├── ArchiveOriginals
│   ├── myd_ncov421_close_ao.mp4
│   └── myd_ncov421_wide_ao
│       └── XDROOT
│           └── ...   
├── EditMasters
│   └── myd_ncov421_em.mov
└── ServiceCopies
    └── myd_ncov421_sc.mp4
    ├── myd_ncov421_close_sc.mp4
    └── myd_ncov421_wide_sc.mp4    
```


## Example with all required and optional elements

(to be reworded)
The following is an example file structure of a performance recorded with a Sony camera capturing to XAVC and a GoPro capturing to its native format. This file structure uses required and optional file classes.  

```
ncov421
├── ArchiveOriginals
│   ├── myd_ncov421_close_ao.mp4
│   └── myd_ncov421_wide_ao
│       └── XDROOT
│           └── ...   
├── EditMasters
│   ├── myd_ncov421_em.srt
│   └── myd_ncov421_em.mov
└── ServiceCopies
    ├── myd_ncov421_sc.srt
    ├── myd_ncov421_sc.mp4
    ├── myd_ncov421_close_sc.mp4
    └── myd_ncov421_wide_sc.mp4      

```
