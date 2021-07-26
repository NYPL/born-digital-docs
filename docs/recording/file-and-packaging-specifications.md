---
layout: default
title: File and Packaging Specifications
nav_order: 0
parent: Recording
---

The document outlines the specifications for born-digital media recorded for NYPL's collections.

## File Classes

Specifications for every file depend on its purpose. NYPL recognizes 4 class of media files.

* Archive Original (AO): The raw files as exported from the recording device. For example, a AVCHD package or H264/MOV.
* Edit Masters (EM): A single file created from editing together the output of the recording devices and adding information such as titles and credits. For example, a single MOV that cuts together wide shots, close shots, titles, and credits.
* Service Copies (SC): Single files transcoded from each of the Archive Originals and Edit Master files. For example, an MP4 of the AO AVCHD example above.
* Images (Optional): still images captured to accompany the audio or video documentation
* Project Files (Optional): files created by NLEs to manage the composition of timelines
* Captions (Optional): Timed transcripts of the audio.
* Transcripts (Options): Untimed transcripts of the audio.

## File Names

Filenames must follow consistent across all files. For folder-based formats like AVCHD, original file names within the folder should be left unaltered and the top-level folder should be named in accordance with the rules below about filenames.

### General rules

* Filenames must only use the following characters A-Z, a-z, 0-9, and \_.
* Filenames should only use lowercase characters.
* Filenames should not include spaces: in lieu of spaces, use underscores (\_).

Every filename should begin with the same prefix.

### Structure and order of filename elements

The structure of file names is as follows:
divisioncode_contentcode_purposecode_suffix.extension

* Division Code (required): Filenames should begin with a 3-digit NYPL division code. Division codes are as follows:
  * mao - Manuscripts and Rare Books Division
  * myd - Jerome Robbins Dance Division
  * myh - Rodgers & Hammerstein Division
  * mym - Music Division
  * myt - Theater Division (includes TOFT)

* Content Name (required): Filenames must contain a code unique to the recording. If a classmark has been provided by the library, this should be included as a single, unspaced term. For examle, NCOV 421 becomes ncov421. If there is no classmark, a code be created using the date of recording in yyyymmdd format and a reference to the content. For example, 20210431hellodolly.

* Purpose Code (for AOs, EMs, SCs, Images): Archive Originals and their service copies should include a short phrase to describe their contents. There is no controlled vocabulary but suggested terms include as wide, close, interviewer, subject, gopro, or similar. For example, myt_ncov421_wide_pm.mov.

* Suffix: Filenames must include one of the following suffixes immediately before the extension:
  * ao - archive originals
  * em - edit masters
  * sc - service copies

Some examples of filenames using all elements of this filenaming specification in order:

* myt_ncov421_wide_ao - folder containing the AVCHD files for the wide shot of acquisition ncov421 by the Dance division
* myt_ncov421_wide_pm.mov - video file created from the archive original of the wide shot of acquisition ncov421 by the Dance division
* myt_ncov421_em.mov - video edited together from all camera shots for acquisition ncov421 by the Dance division
* myt_ncov421_wide_sc.mp4 - video derived from the wide shot of acquisition ncov421 by the Dance division
* myt_ncov421_sc.mp4 - video derived from the the edit master for acquisition ncov421 by the Dance division
* myt_ncov421_sc.srt - a caption file for the audio of the service file
* myt_ncov421_interviewee.jpeg - image of the interview subject for acquistion ncov421 by the Dance division
* myt_ncov421.prproj - the Adobe Premiere project file for creating the edit from elements

## Format Specifications

The following specifications represent baseline requirements for file formats. Additional formats and codecs may be added upon request after consulting with Digital Preservation, PAMI, and curatorial staff.

## Video Format Specifications

### Archive Original Video Files

Archive original files should use whatever formats are native to the recording equipment with specifications that meet curatorial needs.

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  -----------  |
|  Container  |  Camera Native (e.g. AVCHD, XAVC, MPEG-2, MOV)  |  -  |
|  Video Codec  |  Camera Native (H.264, MPEG-4)  |  |
|  Chroma Subsampling  |  4:2:2 or greater  |  4:2:0  |
|  Bit Depth  |  10 bit or greater  |  8 bit  |
|  Bit Rate  |  20 Mbps or greater  |  5 Mbps or greater  |
|  Frame Rate  |  29.97 fps or greater  |  24 fps  |
|  Frame Size  |  1080P or greater  |  720p  |
|  Audio Codec  |  PCM, AC-3, AIFF  |  -  |
|  Audio Bit Depth  |  16 bit or greater  |  -  |
|  Audio Sampling Rate  |  44.1 kHz or greater  |  -  |
|  Audio Channels  |  Stereo Pair  |  -  |

### Edit Master Video Files

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  -----------  |
|  Container  |  MOV  |  MXF  |
|  Video Codec  |  ProRes 422 HQ or greater, DNxHD220x or greater  |  ProRes, DVCPro HD, XDCAM, Cineform  |
|  Chroma Subsampling  |  4:2:2 or greater  |  4:2:0  |
|  Bit Depth  |  10 bit or greater  |  8 bit  |
|  Bit Rate  |  Matched to Archive Original  |  5 Mbps or greater  |
|  Frame Rate  |  Matched to Archive Original  |  29.97 FPS or greater  |
|  Frame Size  |  Matched to Archive Original  |  720P or greater  |
|  Audio Codec  |  PCM, AC-3, AIFF  |  -  |
|  Audio Bit Depth  |  Matched to Archive Original  |  16 bit or greater  |
|  Audio Sampling Rate  |  Matched to Archive Original  |  44.1 kHz or greater  |
|  Audio Channels  |  Stereo Pair, Dolby  |  -  |

### Service File Video Files

Service files should not be upsampled if their source files are under spec.

|  Attribute  |  Spec  |
|  -----------  |  -----------  |
|  Container  |  MP4  |
|  Video Codec  |  H.264  |
|  Bit Rate  |  8 mbps or greater  |
|  Frame Rate  |  29.97 FPS  |
|  Frame Size  |  1080P  |
|  Audio Codec  |  AAC  |
|  Audio Bit Rate  |  256 kbps  |
|  Audio Channels  |  Stereo Pair  |

## Audio Format Specifications

### Archive Original Audio Files

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  -----------  |
|  Container  |  Recorder Native (WAV, M4A, MP3)  |  -  |
|  Audio Codec  |  Recorder Native (PCM, AC3, AAC, MP3, FLAC)  |  -  |
|  Bit Depth  |  Recorder Native (16 bit or more)  |  -  |
|  Sampling Rate  |  Recorder Native (44.1 kHz or more)  |  -  |
|  Bit Rate  |  Recorder Native  (192 kbps or more)  |  128 kbps  |
|  Audio Channels  |  Recorder Native (Mono, Stereo) |  -  |

### Edit Master Files

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  -----------  |
|  Container  |  WAV or Matched to Archive Original  |  -  |
|  Audio Codec  |  PCM or Matched to Archive Original  |  -  |
|  Bit Depth  |  16 bit, 24 bit  |  -  |
|  Sampling Rate  |  44.1, 48, or 96 kHz  |  -  |
|  Bit Rate  |  Matched to Archive Original  |  128 kbps  |
|  Audio Channels  |  Recorder Native, Stereo Pair  |  -  |

### Service Copy Audio Files

Service files should not be upsampled if their source files are under spec.

|  Attribute  |  Spec  |
|  -----------  |  -----------  |
|  Container  |  MP4 (M4A)  |
|  Video Codec  |  AAC  |
|  Bit Rate  |  192 kbps  |
|  Audio Channels  |  Stereo Pair  |

### Image Files

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  ----------  |
|  File Format  |  JPEG  |  HEIF  |
|  Resolution  |  5 MP or greater  |  -  |

### Caption Files

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  ----------  |
|  File Format  |  WebVTT  |  SRT, SSA, ASS  |
|  Text Encoding  |  UTF-8  |  -  |

### Transcript Files

|  Attribute  |  Preferred Spec  |  Accepted  |
|  -----------  |  -----------  |  ----------  |
|  File Format  |  PDF  |  -  |
|  Text Encoding  |  UTF-8  |  -  |

## Packaging Files

Files must be organized according to the structure

* {Content Name}
  * ArchiveOriginals
  * EditMasters
  * ServiceCopies
  * Images

There should be no additional folders.

## Examples

The following is an example of a performance recorded with a Sony camera capturing to XAVC and a GoPro capturing to its native format.

* ncov421
  * ArchiveOriginals
    * myt_ncov421_wide_ao
      * XDROOT
    * myt_ncov421_close_ao.mp4
  * EditMasters
    * myt_ncov421_em.mov
    * myt_ncov421_em.srt
  * ServiceCopies
    * myt_ncov421_wide_sc.mp4
    * myt_ncov421_close_sc.mp4
    * myt_ncov421_sc.mp4
    * myt_ncov421_sc.srt
  * Images
    * myt_ncov421_titlecard.jpeg
  * ProjectFiles
    * myt_ncov421.prproj

The following is an example of an oral history captured using a cellphone app.

* 20210223interviewjanedoe
  * ArchiveOriginals
    * mao_20210223interviewjanedoe_primary_ao.mp3
    * mao_20210223interviewjanedoe_backup_ao.mp3
  * EditMasters
    * mao_20210223interviewjanedoe_em.mp3
  * ServiceCopies
    * mao_20210223interviewjanedoe_primary_sc.mp3
    * mao_20210223interviewjanedoe_backup_sc.mp3
    * mao_20210223interviewjanedoe_sc.mp3
    * mao_20210223interviewjanedoe_transcript.pdf
  * Images
    * mao_20210223interviewjanedoe_portrait.jpeg
    * mao_20210223interviewjanedoe_interviewer.jpg

Once organized according to this structure, files should be bagged according to the Library of Congress BagIt File Packaging Format. Specific instructions on how to bag files may be found in [Bagging Files](bagging-files) for submission.
