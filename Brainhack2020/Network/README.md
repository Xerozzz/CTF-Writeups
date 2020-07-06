# Network

##  Network-1 Baby Shark
### Challenge
Recently the Resistance Fighters have discovered this new thing called Wireshark, it seems to be some kind of tool used for analysing network packets.

We tried to capture a little snippet of traffic while browsing the web just to check out its capabilities. Let's check out what it can do.

MD5("easy.pcap"): aa16be8f7032586d5bfc675e9ac8e982

### Solution
When opening the file with WireShark, I went to export all HTTP objects immediately, using File > Export > HTTP. There was a file called "Confidential.pdf" which contained the flag when opened

### Flag
CDDC20{TLP_RED_EYES_ONLY}

## Network-2 Mama Shark
### Challenge
We have received a new packet for analysis.

Oh damn, there's too much more traffic to look through.. Is there a shortcut to find what we're looking for immediately?

MD5("noisy.pcap"): dabae618e77eb2532d1215700deaffdc

### Solution
After opening the WireShark file, I exported all HTTP objects again. Locate the file called "yumcheese.txt" and use "Control+F" for the flag.

### Flag
CDDC20{JUST_GIVE_ME_TL:DR}