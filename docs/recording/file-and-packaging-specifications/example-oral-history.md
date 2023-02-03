---
layout: default
title: Example Oral History Package
parent: File and Packaging Specifications
grand_parent: Recording
nav_order: 4
---

## Example Oral History Package Specifications
The page outlines file and packaging specifications for Oral History collections. These specifications assume the oral histories in question are audio files. For oral histories including video consult the package specifications for [Dance Oral Histories](https://nypl.github.io/born-digital-docs/docs/recording/file-and-packaging-specifications/example-DOH.html) as an example and contact [Digital Preservation](mailto:digitalarchives@nypl.org) for specific guidance applicable to your division policies.

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

The following is an example file structure of an oral history. File names should be consistent across all files and follow division_nameofinterviewee_subcomponent_type convention where "subcomponent" may describe parts (a recording was completed in parts) or dates (a recording was completed across different dates). For detailed file name conventions consult the [File and Packaging Specifications](https://nypl.github.io/born-digital-docs/docs/recording/file-and-packaging-specifications/file-and-packaging-specifications.html#file-names) guide.

```
nameofinterviewee 
├── EditMasters
│   └── mao_nameofinterviewee_part1_em.wav
│   └── mao_nameofinterviewee_part2_em.wav
├── ServiceCopies
│   └── mao_nameofinterviewee_part1_sc.m4a 
│   └── mao_nameofinterviewee_part2_sc.m4a 
└── Transcripts
    └── mao_nameofinterviewee_part1_transcript.pdf
    └── mao_nameofinterviewee_part2_transcript.pdf
```

## Example oral history package including optional elements

The following is an example file structure of an oral history adding optional elements to minimum requirements.

```
nameofinterviewee
├── ArchiveOriginals
│   ├── mao_nameofinterviewee_part1_ao.wav 
│   └── mao_nameofinterviewee_part2_ao.wav  
├── EditMasters
│   └── mao_nameofinterviewee_part1_em.wav
│   └── mao_nameofinterviewee_part2_em.wav
├── ServiceCopies
│   └── mao_nameofinterviewee_part1_sc.m4a 
│   └── mao_nameofinterviewee_part2_sc.m4a 
├── Transcripts
│   └── mao_nameofinterviewee_part1_transcript.pdf
│   └── mao_nameofinterviewee_part2_transcript.pdf
└── Releases
    └── mao_nameofinterviewee_part1_release.pdf
    └── mao_nameofinterviewee_part2_release.pdf
    
```