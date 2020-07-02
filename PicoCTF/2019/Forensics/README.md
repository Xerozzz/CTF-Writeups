#  Forensics

## Things you need


## Glory of the Garden (50 points)
### Challenge
This garden contains more than it seems. You can also find the file in /problems/glory-of-the-garden_6_0d6d3ea97757b84c7a51a38daa7dca8d on the shell server.

### Solution
The hint for this challenge said "Hex Editor". I googled for a hex editor at HexEd.it and looked at the hex dump. At the bottom line you can see the flag in clear view.

### Flag
picoCTF{more_than_m33ts_the_3y3f20F5be9}

## unzip (50 points)
### Challenge
Can you unzip this file and get the flag?

### Solution
Download the zip file and extract it. You will see a .png file in it. Open it, the flag is there, just wrap it with "picoCTF{}".

### Flag
picoCTF{unz1pp1ng_1s_3a5y}

## So Meta (150 points)
### Challenge
Find the flag in this picture. You can also find the file in /problems/so-meta_1_ab9d99603935344b81d7f07973e70155.

### Solution
Put the picture into a Linux machine and run the strings command on it. The flag should be visible at the bottom few lines.

### Flag
picoCTF{s0_m3ta_368a0341}

## What Lies Within (150 points)
### Challenge
Theres something in the building. Can you retrieve the flag?

### Solution
The name sounds very suspiciously like a steganography challenge. To start, I googled Steganography Online and used the web decoder. I selected the buildings.png and decoded it. On the first like is the flag.

### Flag
picoCTF{h1d1ng_1n_th3_b1t5}

## extensions (150 points)
### Challenge
This is a really weird text file TXT? Can you find the flag?

### Solution
The name is a giveaway already. I googled a hex editor, HexEd.it and inserted the file. The file header does not look like a txt file. I googled the file header "89 50 4E 47" and it showed png, so i changed the extension from .txt to .png and the flag was there. <br>Alternatively, if you open the .txt file, you can see that there is a png at the top, a huge hint.

### Flag
picoCTF{now_you_know_about_extentions}

## shark on wire (150 points)
### Challenge
We found this packet capture. Recover the flag. You can also find the file in /problems/shark-on-wire-1_0_13d709ec13952807e477ba1b5404e620.

### Solution
What we have here is a .pcap file. You can use a free open-source tool called Wireshark to open it. After opening it with Wireshark, we can see many packets, in particular, UDP packets. The hint said "streams" so I used "udp.stream eq" and did 1, 2, 3 so and so forth. I went to follow the UDP stream for each of these. At "udp.stream eq 6", the flag can be seen.

### Flag
picoCTF{StaT31355_636f6e6e}

## WhitePages (250 points)
### Challenge
I stopped using YellowPages and moved onto WhitePages... but the page they gave me is all blank!

### Solution


### Flag

## c0rrupt (250 points)
### Challenge
We found this file. Recover the flag. You can also find the file in /problems/c0rrupt_0_1fcad1344c25a122a00721e4af86de13.

### Solution


### Flag

## like1000 (250 points)
### Challenge
This .tar file got tarred alot. Also available at /problems/like1000_0_369bbdba2af17750ddf10cc415672f1c.

### Solution
When unzipping 1000.tar, it came out as 999.tar. After unzipping that, it became 998.tar. Hence, I assumed the tar files were all numerical order. We can use a linux shell script to untar this. Create a .sh file with the following code:

```
#!/bin/bash
for ((i=1000;i>0;i--));do
    if [ i -f "$i.tar" ] ; then
        break
    fi
    tar -xvf $i.tar
    rm $i.tar
done
cd..
```

It will then review a flag.png, open that for the flag.

### Flag
picoCTF{l0t5_0f_TAR5}

## m00nwalk (250 points)
### Challenge
Decode this message from the moon. You can also find the file in /problems/m00nwalk_1_727ca48dac5da21d2c11635238649314.

### Solution
If you google and research a bit, you can find out that this is an audio recording that transmits SSTV signals. Download a SSTV decoder software and try the various options. The correct option is "Scottie 1" and BPF only. It will then load an image which contains the flag which is upside down

### Flag
picoCTF{beep_boop_im_in_space}

