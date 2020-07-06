# Forensics

## Forensics-1 Can't See A Thing
### Challenge
What kind of lousy photographer takes terrible pictures like these?

MD5("img.jpg"): 4bdba9f047cb651b3645cfe6a41666ba

### Solution
Download the .jpg file and put it into Jeffrey Friedl's Image Metadata Viewer to find out some info. You should see "02CDDC{yhp4rg07ohp_5i_EmOs3wa}" in the XP Comment. Reverse each word individually and reorder the "CDDC20" to get something like "photography is awesome" but in that weird format they gave. Thats the flag

### Flag
CDDC20{pho70gr4phy_i5_aw3sOmE}


## Forensics-2 Shell History

### Challenge
DESCRIPTION
What happened to my server? Please help me to investigate.

Username: root / Password: toor

You don't need to download everything, please use only 1 link.
DOWNLOAD 1   (https://drive.google.com/file/d/1QOiQtZqtGrNFb9ISbo_5cXP0vdZIvaLa/view)
DOWNLOAD 2
DOWNLOAD 3
DOWNLOAD 4
DOWNLOAD 5

MD5("Shell History.ova"): 051736c88e59eb57e3a1fff65ffa40e8

ATTACHED FILES
None

### Solution
Download the any one of the files, open .ova file using Virtual Box, login and type command 'history'. Flag will be displayed.

### Flag
CDDC20{Sh4LL_we_Sh3LL?}

# Forensics-3 TopSecret

## Challenge

## Solution
Use FTK Imager to open the TopSecret file given, but rename it to "TopSecret.ad1" first. AFter that, export all objects and take a look at the text file. It contains lorem ipsum. Use control+F to find the flag

## Flag
CDDC20{Lorem-Ipsum-Foo-Bar}
