# Reverse Engineering

## [RE (Windows)-1] Decompile Me

### Challenge

Hello py2exe, nice to meet you!

MD5("DecompileMe.zip"): 3805ccecd327d3cfcfdcc12c1ce7891b

### Solution

Install unpy2exe, run ` py -2 unpy2exe (without the .py) -o OUTPUT_DIR -v filename ` to get the pyc file. I then cloned the git repo for REpdb and ran ` python2.7 REpdb.py ` to decompile the pyc file.

### Flag

CDDC20{NiCe-2-MeeT-py2exe~:D}

## Dissect Me

### Challenge

LET THE GAMES BEGIN!

### Solution

Download 7zip [here](https://www.7-zip.org/download.html), open it, select DissectMe.exe, and extract out its contents. The path to the flag is DissectMe\.rsrc\0\BITMAP.

### FLag

CDDC20{UR-di$$ector}