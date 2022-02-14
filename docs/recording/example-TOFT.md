---
layout: default
title: Example TOFT Package
nav_order: 0
parent: File and Packaging Specifications
---

## Example TOFT Package Specifications
The document outlines file and packaging specifications for recording for TOFT. If you have questions about the specifications please contact [Digital Preservation](mailto:digitalarchives@nypl.org) staff for guidance.

## File Classes

* Archive Original (AO): (Required)
* Edit Masters (EM): (Required)
* Service Copies (SC): (Required ONLY for Edit Masters)
* Images: (N/A)
* Project Files (Optional): (N/A)
* Captions: Maybe
* Transcripts: (N/A)

## Example with only required elements

(to be reworded)
The following is an example file structure of a performance recorded with a Sony camera capturing to XAVC and a GoPro capturing to its native format. This file structure uses just required file classes. 

```
ncov421
├── ArchiveOriginals
│   ├── myt_ncov421_close_ao.mp4
│   └── myt_ncov421_wide_ao
│       └── XDROOT
│           └── ...   
├── EditMasters
│   └── myt_ncov421_em.mov
└── ServiceCopies
    └── myt_ncov421_sc.mp4
```


## Example with all required and optional elements

(to be reworded)
The following is an example file structure of a performance recorded with a Sony camera capturing to XAVC and a GoPro capturing to its native format. This file structure uses required and optional file classes.  

```
ncov421
├── ArchiveOriginals
│   ├── myt_ncov421_close_ao.mp4
│   └── myt_ncov421_wide_ao
│       └── XDROOT
│           └── ...   
├── EditMasters
│   ├── myt_ncov421_em.srt
│   └── myt_ncov421_em.mov
└── ServiceCopies
    ├── myt_ncov421_sc.srt
    └── myt_ncov421_sc.mp4

```