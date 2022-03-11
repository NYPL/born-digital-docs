---
layout: default
title: Example DOH Package
parent: File and Packaging Specifications
grand_parent: Recording
nav_order: 3
---

## Example DOH Package Specifications
The document outlines file and packaging specifications for recording for Dance Oral Hisotry Program (DOH). 
If you have questions about the specifications please contact [Digital Preservation](mailto:digitalarchives@nypl.org) staff for guidance.

## File Classes

* Archive Original (AO): **Required**
* Edit Masters (EM): **Required**
* Service Copies (SC): **Required for Edit Masters** 
* Images: Optional
* Project Files: N/A
* Captions: Optional
* Transcripts: Optional

## Example with audio oral history with minimum required elements

The following is an example file structure of an oral history recorded in person. 

```
nameofinterviewee
├── ArchiveOriginals
│   └── myd_nameofinterviewee_ao.wav  
├── EditMasters
│   └── myd_nameofinterviewee_em.wav
├── ServiceCopies
│   └── myd_nameofinterviewee_sc.m4a 
└── Images
    └── myd_nameofinterviewee_headshot.jpeg
```


## Example with video oral history with minimum required elements

The following is an example file structure of an oral history recorded via web conferencing software.  

```
nameofinterviewee
├── ArchiveOriginals
│   ├── myd_nameofinterviewee_portrait_ao.mp4
│   └── myd_nameofinterviewee_gallery_ao.mp4  
├── EditMasters
│   └── myd_nameofinterviewee_em.mp4
├── ServiceCopies
│   └── myd_jonathan_sc.mp4 
└── Images
    └── myd_nameofinterviewee_headshot.jpeg
```