---
layout: default
title: How to use BagIt/Bagger
nav_order: 4
parent: Recording
---
# How to use BagIt to package born-digital audiovisual files

**BagIt** is a hierarchical file packaging format designed to support disk-based storage and network transfer of arbitrary digital content. 

Do not bag your project until all edits are made and approved and files are ready to be transferred to NYPL.

The amount of time needed for a bag to be created, will depend on the speed and throughput of your workstation and the storage device you are using. We recommend either bagging files when they are stored on a solid state disk (internal or external) or running the bag process overnight. For reference, creating bags for a 4TB project would take about 30 minutes on a solid state disk or about 4 hours on a hard drive.

## Arrange the files into folders

Files must be organized according to the specified directory structure. For more information on this specification, please refer to the Born Digital Documentation: File and Packaging Specifications page. There should not be additional folders than those outlined below.

- {Content Name}
  - ArchiveOriginals
  - EditMasters
  - ServiceCopies
  - Images

## Instructions to use Bagger, the BagIt Graphical User Interface:
These instructions assume that you have Bagger installed on your workstation, if that’s not the case go to the Install Bagger instructions.

1. Open Bagger
2. Click on ‘Create bag in place’ on the top menu bar
3. In the dialog box, navigate to the directory where your files are located on the ‘Select data’ field
4. Select ‘no profile’ and click ‘OK’
5. After the dialog box confirms that a bag was created successfully, verify the bag by clicking on the ‘Is Bag Complete’ section on the top main menu. 
6. If bag is complete, move the bag to the transfer storage device (G-drive or external hard-drive)

## Alternative: Instructions to use bagit-python, the BagIt Command Line Interface:
These instructions assume that you have bagit-python installed on your workstation, if that’s not the case go to the Install bagit-python instructions.

1. Open your terminal
2. Enter the following, including the final space, `bagit.py --md5 ` and then either drag-and-drop the folder icon for the directory where your files are located or type in the path for that directory
3. After the process finishes, verify the bag by running the following command `bagit.py --validate --completeness-only /path/to/bag/`
4. If bag is complete, move the bag to the transfer storage device (G-drive or external hard-drive)
