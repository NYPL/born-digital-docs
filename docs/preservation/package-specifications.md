---
layout: default
title: Package Specifications
parent: Preservation
nav_order: 4
---

Several derivative packages are created from a received package of born-digital audio and moving image material.
These are in two categories, edit packages and original packages.

## Edit Packages

Edit packages must contain the original edit and service files submitted.
If necessary, these files may be edited according to the (processes documented here)[updating-received-files]

```sh
folder_name
├── bag-info.txt
├── bagit.txt
├── data
│   ├── EditMasters
│   │   └── div_classmark_em.mov
│   └── ServiceCopies
│       └── div_classmark_sc.mp4
└── manifest-md5.txt
```

Optional files that support the edit such as captions and transcripts should be included in this package

## Original Packages

Original packages must contain only one of the archive original videos and an associated service file.
Any production may have multiple original packages.
If necessary, these files may be edited according to the (processes documented here)[updating-received-files].
This often includes creating a service file and rewrapping complex video formats to single files.

```sh
folder_name
├── bag-info.txt
├── bagit.txt
├── data
│   ├── ArchiveOriginals
│   │   └── div_classmark_close_ao.mkv
│   └── ServiceCopies
│       └── div_classmark_close_sc.mp4
└── manifest-md5.txt
```
