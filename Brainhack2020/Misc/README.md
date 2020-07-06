# Misc

## Misc-1 Welcome to CDDC 2020
### Challenge
Free points for all! See you on Slack! ;)

### Solution
Go to the announcements channel in Slack, click "Details" at the top right corner and click About. The flag is there

### Flag
CDDC20{g1mM3_M0aRRr_pOiN75}

## Misc-2 ARGH
### Challenge
I found a binary, together with this long string that looks like some password. I wonder what is it for...

Key: GZ2gXZ3bD2qqNyNxXb5LJ8HfHQtTL5VHA

MD5("myprog"): e6c76a1dbc54005fdd2c1203e117d514

### Solution


### Flag


## Visual Noise

### Challenge

I intercepted some emails from Unduplicitous Corp, that had these pictures attached to them. Looks like visual noise but then again, I can't be sure....

MD5("so-noisy.png"): 0ec6ae0ccba7aa6e9a5726b186bcde9e
MD5("much-confusing.png"): aa685b5a77aae415cc85ae0dcb8048d3

### Solution

Used [an online tool](https://www.diffchecker.com/image-diff) to compare the 2 PNG files.

### Flag

CDDC20{V1suAl_CrYPT0_iS_s0_53cuRE}

## Recycling Bin

### Challenge 

Found this file in one of the Unduplicitous Corp's PCs Recycle Bin. Can you walk me through this?

### Solution



### Flag

CDDC20{cArv3_C4Rve_CaRV33eE}

## ilovedes

### Challenge

I heard that the CFO of Unduplicitous Corp loves using DES to encrypt his data, LOL.

### Solution

Using an [online tool](http://des.online-domain-tools.com/), you can decode the secret.dat file with the key "ilovedes".

### Flag

CDDC20{i_l0v3_5yMmetR1c_EnCryp7i0N}

## How QueeR...

### Challenge
We reailsed that Unduplicitous Corp uses this code for their assets tagging. But we can't figure out how exactly to decode it, hmm.

MD5("barcode.gif"): df90bf8d0533e5757ea1fede8743adbc

## Solution
Inverse the colors of the gif using any image editing tool, then put it into a barcode scanner to get the flag

### Flag
CDDC20{Qu1Rky_quEeR_qUe57ion4bL3_c0d35s}
