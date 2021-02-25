---
layout: default
title: File and Packaging Specifications
nav_order: 1
parent: Recording
---

## File Classes

Specifications for every file depend on its purpose. NYPL recognizes 4 class of media files.

* Archive Original (AO): The raw files from the recording device. For example, a BPAV package.

* Preservation Masters (PM): A single file created from the output of a single recording device. For example, a single MOV created from the set of M2TS files produced by a Sony camera.

* Edit Masters (EM): A single file created from editing together the output of the recording devices and adding information such as titles and credits. For example, a single MOV that cuts together wide shots, close shots, titles, and credits.

* Service Copies (SC): Single files transcoded from each of the Preservation and Edit Master files. For example, an MP4 of the Preservation Master MOV example above.

* Images: still images captured to accompany the audio or video documentation

## File Names
Filenames must follow consistent across all files. For file-based formats like AVCHD, original file names should be left unaltered and contained in a single folder named in accordance with the rules below about filenames.

### General rules

* Filenames must only use the following characters A-Z, a-z, 0-9, and \_.
* Filenames should be in lowercase characters only.
* Filenames should not include spaces: in lieu of spaces, use underscores (\_).

Every filename should begin with the same prefix.
Structure and order of filename elements
The structure of file names is as follows:
divisioncode_acquisitionid_content_suffix.extension

* Division Code (required): Filenames should begin with a 3-digit NYPL division code. Division codes are as follows:
	* myd - Jerome Robbins Dance Division
	* myt - Theater Division (includes TOFT)
	* mym - Music Division
	* myh - Rodgers & Hammerstein Division

* Acquisition ID (required): Filenames must include the 4-digit acquisition number provided to recorders in the metadata Google Sheet shared with them by the curatorial division.

* Content (for AOs, PMs, SCs, Images): Preservation masters and their service copies should include a short phrase to describe their contents. There is no controlled vocabulary but suggested terms include as wide, close, interviewer, subject, gopro, or similar. For example, myd_1111_wide_pm.mov.

* Suffix: Filenames must include one of the following suffixes immediately before the extension:
	* ao - archive originals
	* pm - preservation masters
	* em - edit masters
	* sc - service copies

Some examples of filenames using all elements of this filenaming specification in order:
* myd_1111_wide_ao - folder containing the AVCHD files for the wide shot of acquisition 1111 by the Dance division
* myd_1111_wide_pm.mov - video file created from the archive original of the wide shot of acquisition 1111 by the Dance division 
* myd_1111_em.mov - video edited together from all camera shots for acquisition 1111 by the Dance division 
* myd_1111_wide_sc.mp4 - video derived from the wide shot of acquisition 1111 by the Dance division 
* myd_1111_sc.mp4 - video derived from the the edit master for acquisition 1111 by the Dance division 
* myd_1111_interviewee.jpeg - image of the interview subject for acquistion 111 by the Dance division

## Format Specifications
The following specifications represent baseline requirements for file formats. Additional formats and codecs may be added upon request after consulting with Digital Preservation, PAMI, and curatorial staff.

## Video Format Specifications

### Archive Original Video Files
| Attribute | Preferred Spec | Accepted |
| ----------- | ----------- |
| Container      | AVCHD      | MXF |
| Video Codec      |  | |
| Chroma Subsampling      | 4:2:2 or greater       | 4:2:0 |
| Bit Depth      | 10 bit or greater      | 8 bit |
| Bit Rate      | Camera Native      | 30mbps or greater |
| Frame Rate     | Camera Native       | 29.97 FPS or greater |
| Frame Size      | Camera Native      | 1080P or greater |
| Audio Codec      | PCM, AC-3, AIFF      | - |
| Audio Bit Depth | 16 or 24 bit      | - |
| Audio Sampling Rate    | 44.1 or 48 kHz      | - |
| Audio Channels   | Stereo Pair |  - |

### Preservation and Edit Master Video Files
| Attribute | Preferred Spec | Accepted |
| ----------- | ----------- |
| Container      | MOV      | MXF |
| Video Codec      | ProRes 422 HQ or greater, DNxHD220x or greater     | ProRes, DVCPro HD, XDCAM, Cineform |
| Chroma Subsampling      | 4:2:2 or greater       | 4:2:0 |
| Bit Depth      | 10 bit or greater      | 8 bit |
| Bit Rate      | Camera Native      | 30mbps or greater |
| Frame Rate     | Camera Native       | 29.97 FPS or greater |
| Frame Size      | Camera Native      | 1080P or greater |
| Audio Codec      | PCM, AC-3, AIFF      | - |
| Audio Bit Depth | 16 or 24 bit      | - |
| Audio Sampling Rate    | 44.1 or 48 kHz      | - |
| Audio Channels   | Stereo Pair, Dolby |  - |

### Service Copy Video Files
| Attribute | Spec |
| ----------- | ----------- |
| Container      | MP4      |
| Video Codec      | H264 |
| Bit Rate      | 10 mbps or greater |
| Frame Rate     | 29.97 FPS | 
| Frame Size      | 1080P |
| Audio Codec      | AAC |
| Audio Bit Rate | 256 kbps |
| Audio Channels   | Stereo Pair |

## Audio Format Specifications

### Archive Original Audio Files

| Attribute | Preferred Spec | Accepted |
| ----------- | ----------- | ----------- |

### Preservation/Edit Master Files

| Attribute | Preferred Spec | Accepted |
| ----------- | ----------- | ----------- |
| Container      | WAV      | WAV, FLAC, MP3 |
| Video Codec      | PCM | PCM, AC3, AAC, MP3, FLAC |
| Bit Depth | 16 bit, 24 bit      | - |
| Sampling Rate    | 44.1, 48, or 96 kHz      | - |
| Bit Rate | 192 kbps | 128 kbps | - |
| Audio Channels   | Recorder Native, Stereo Pair | - |

### Service Copy Audio Files
| Attribute | Spec |
| ----------- | ----------- |
| Container      | MP3, MP4 (M4A)      |
| Video Codec      | MP3, AAC |
| Bit Rate      | 192 kbps |
| Audio Channels   | Stereo Pair |

### Image Files
| Attribute | Preferred Spec | Accepted |
| ----------- | ----------- | ---------- |
| File Format      | JPEG      | HEIF |
| Resolution | 5 MP or greater| - |

## Packaging Files

Files must be organized according to the structure

* {Acquisition ID}
	* ArchiveOriginals
	* PreservationMasters
	* EditMasters
	* ServiceCopies
	* Images

There should be no additional folders. As an example:

* 1111
	* ArchiveOriginals
		* myd_1111_wide_ao
			* PRIVATE
			* DCIM
			* MISC
		* myd_1111_close_ao
			* PRIVATE
			* DCIM
			* MISC
	* PreservationMasters
		* myd_1111_wide_pm.mov
		* myd_1111_close_pm.mov
	* EditMasters
		* myd_1111_em.mov
	* ServiceCopies
		* myd_1111_wide_sc.mp4
		* myd_1111_close_sc.mp4
		* myd_1111_sc.mp4
	* Images
		* myd_1111_interviewee.jpeg

Once organized according to this structure, files should be bagged according to the Library of Congress BagIt File Packaging Format. Specific instructions on how to bag files may be found in [Bagging Files for Submission]().
