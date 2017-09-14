# ImageTrove python DICOM uploader

Andrew Janke - __andrew.janke@uq.edu.au__ - National Imaging Facility.


Auto-upload from instrument to an AAF authenticated ImageTrove/MyTardis respository (in NecTAR/AWS cloud) from an instrument. Works by watching a local dcmtk DICOM listener client that runs in the local network. Thus it can upload data past VPN's and all sorts of hard things has it only uses the HTTPS protocol. All data is identified by project (and thus a group of people) from there access to the data is granted to the group of users associated with the project. 

## Usage
This python listener client will connect to a single instance of Imagetrove/MyTardis but can back-end on multiple DICOM instruments (typically MRI/CT/PET).
