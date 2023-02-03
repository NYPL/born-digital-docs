---
layout: default
title: Example Oral History Package
parent: File and Packaging Specifications
grand_parent: Recording
nav_order: 4
---

## Example Oral History Package Specifications
The page outlines file and packaging specifications for Oral History collections. These specifications assume the oral histories in question are audio files. For oral histories including video, consult the package specifications for [Dance Oral Histories](https://nypl.github.io/born-digital-docs/docs/recording/file-and-packaging-specifications/example-DOH.html) If you have questions about the specifications please contact [Digital Preservation](mailto:digitalarchives@nypl.org) staff for guidance.

## File Classes

* Archive Original (AO): Optional
* Edit Masters (EM): **Required**
* Service Copies (SC): **Required for Edit Masters** 
* Images: Optional
* Project Files: N/A
* Captions: Optional
* Transcripts: Optional
* Releases: Optional

## Example oral history package with minimum required elements

The following is an example file structure of an oral history recorded in person.

```
nameofinterviewee 
├── EditMasters
│   └── mao_nameofintervieweepart1_em.wav
│   └── mao_nameofintervieweepart2_em.wav
├── ServiceCopies
│   └── mao_nameofinterviewee_sc.m4a 
└── Transcripts
    └── mao_nameofinterviewee_transcript.pdf
```

## Example oral history package including optional elements

The following is an example file structure of an oral history adding optional elements to minimum requirements.

```
nameofinterviewee
├── ArchiveOriginals
│   ├── mao_nameofintervieweepart1_ao.wav 
│   └── mao_nameofintervieweepart2_ao.wav  
├── EditMasters
│   └── mao_nameofinterviewee_em.wav
├── ServiceCopies
│   └── mao_nameofinterviewee_sc.m4a 
├── Transcripts
│   └── mao_nameofinterviewee_transcript.pdf
└── Releases
    └── mao_nameofinterviewee_release.pdf
```