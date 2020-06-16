# General Skills

## Things you need
- Any linux systems (Kali, Ubuntu etc)
- PicoCTF webshell
- Online converters (Binary, Hex, Decimal, Octal)
- Google
- A lot of patience and curiosity

## Challenges
- [Lets Warm Up (50 points)](##-Lets-Warm-Up-(50points))
- Warmed Up (50 points)
- 2Warm (50 points)
- Bases (100 points)
- First Grep (100 points)
- Resources (100 points)
- Strings it (100 points)
- What's a netcat (100 points)
- Based (200 points)
- First Grep: Part II (200 points)
- Plumbing (200 points)
- Whats-the-difference (200 points)
- music (300 points)
- 1_wanna_b3_a_r0ck5tar (350 points)

## Lets Warm Up (50 points)
### Challenge
If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?

### Solution
Go to a Hex to ASCII converter or use the python script below.

```python
>>> chr(0x70)
'p'
```

### Flag
picoCTF{p}

## Warmed Up (50 points)
### Challenge
What is 0x3D (base 16) in decimal (base 10).

### Solution
Go to a Hex to Decimal converter online or use the python script

```python
>>> 0x3d
61
```

### Flag
picoCTF{61}

## 2Warm (50 points)
### Challenge
Can you convert the number 42 (base 10) to binary (base 2)?

### Solution
Go to a decimal to binary converter online or use the python script below

```python
>>> bin(42)
'0b101010'
```

### Flag
picoCTF{101010}

## Bases (100 points)
### Challenge
What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.

### Solution
Flag is encoded with base64. Use online decoder to convert from base64 back.

### Flag
picoCTF{l3arn_th3_r0p35}

## First Grep (100 points)
### Challenge
Can you find the flag in file? This would be really tedious to look through manually, something tells me there is a better way. You can also find the file in /problems/first-grep_2_04dbf496b78e6c37c0097cdfef734d88 on the shell server.

### Solution
Go to "Shell" on the picoctf platform and login. Use `cd /problems/first-grep_2_04dbf496b78e6c37c0097cdfef734d88` to get to the directory with the file to grep. Then use `cat file | grep picoCTF`to get your flag.

### Flag
picoCTF{grep_is_good_to_find_things_bf6aec61}

## Resources (100 points)
### Challenge
We put together a bunch of resources to help you out on our website! If you go over there, you might even find a flag!

### Solution
Go to the link and scroll down past the video. It's right there. Use the 2019 one.

### Flag
picoCTF{r3source_pag3_f1ag}

## Strings it (100 points)
### Challenge
Can you find the flag in file without running it? You can also find the file in /problems/strings-it_2_865eec66d190ef75386fb14e15972126 on the shell server.

### Solution
Go to "Shell" on the picoctf platform and login. Use `cd /problems/strings-it_2_865eec66d190ef75386fb14e15972126` to get to the directory with the file to find. Run `strings strings | grep picoCTF`

### Flag
picoCTF{5tRIng5_1T_d5b86184}

## What's a netcat (100 points)
### Challenge
Using netcat (nc) is going to be pretty important. Can you connect to 2019shell1.picoctf.com at port 32225 to get the flag?

### Solution
Use the shell provided or your own linux system. Run `nc 2019shell1.picoctf.com 32225` and you will get your flag.

### Flag
picoCTF{nEtCat_Mast3ry_b1d25ece}

## Based (200 points)
### Challenge
To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337? Connect with nc 2019shell1.picoctf.com 31615.

### Solution
Run `nc 2019shell1.picoctf.com 31615` in the shell or your own linux system. They will rapid fire you questions to convert into words. Prepare some binary, hex, octal converters to copy paste quick! Once you get past 3 challenges you get the flag.

### Flag
picoCTF{learning_about_converting_values_502ff297}

## First Grep: Part II (200 points)
### Challenge
Can you find the flag in /problems/first-grep--part-ii_1_4496a9af2273007b52d4a1adec323b76/files on the shell server? Remember to use grep.

### Solution
Go to "Shell" on the picoctf platform and login. Use `cd /problems/first-grep--part-ii_1_4496a9af2273007b52d4a1adec323b76/files` to go to the directory. You will see that you have multiple files if you use `ls`. You can cat each file one by one and use grep like the method for the previous grep challenge, but another way is to use `grep -r picoCTF` to quickly grep through all the folders and their subfiles to find the flag. -r stands for recursive.

### Flag
picoCTF{grep_r_to_find_this_af11356f}

## Plumbing (200 points)
### Challenge
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to 2019shell1.picoctf.com 21957.

### Solution
When you netcat to the given connection, you get spammed by many lines of gibberish. Unless you want to go through them one by one (PLEASE DON'T), you have to save it to a file then use cat on that file. TO do that, use your linux system, and do `nc 2019shell1.picoctf.com 21957 > test.txt`. This will save all that output gibberish to a text file called "test.txt" which will be saved into the directory you are in right now. After that, do `cat test.txt | grep picoCTF` to get your flag.

### Flag
picoCTF{digital_plumb3r_c1082838}

## Whats-the-difference (200 points)
### Challenge
Can you spot the difference? kitters cattos. They are also available at /problems/whats-the-difference_0_00862749a2aeb45993f36cc9cf98a47a on the shell server

### Solution
*WIP*

### Flag
picoCTF{th3yr3_a5_d1ff3r3nt_4s_bu773r_4nd_j311y_aslkjfdsalkfslkflkjdsfdszmz10548}

## where-is-the-file (200 points)
### Challenge
I've used a super secret mind trick to hide this file. Maybe something lies in /problems/where-is-the-file_1_54878e9f5b7db0ddbaf642cdb5c9b3b5.

### Solution
cd into the folder given in the challenge. When you type ls, you may think this file is empty. However, type `ls -a` and you can see that there is a file there called ".cant_see_me". -a is used to check for hidden files and folders.

### Flag
picoCTF{w3ll_that_d1dnt_w0RK_3e782057}

## flag_shop 
### Challenge
There's a flag shop selling stuff, can you buy a flag? Source. Connect with nc 2019shell1.picoctf.com 29250.

### Solution
Download the source code. You can see that "total_cost" is given the variable type "int", which makes it a 4 byte signed integer. If we use an integer overflow attack and enter a large enough number for "number_flags", it will make "total_cost" overflow into a negative number. That would make your "account_balance" skyrocket as the value for "account_balance" is derived from "account_balance - total_cost". Get rich, then buy the actual flag.

### Flag
picoCTF{m0n3y_bag5_783740a8}

## music (300 points)
### Challenge
I wrote you a song. Put it in the picoCTF{} flag format

### Solution
The text file looks really interesting, what if it was a programming language that was not one of the norms? Google esoteric language and you will see rockstar as one of them. Use the rockstar website and input the contents of the textfile there. You will get some numbers starting with "114, 114, 114 ...".

Put these numbers into a converter from decimal to ASCII, and you will get the flag.

This challenge requires a bit of guesswork, googling and experience if you are new.

### Flag
picoCTF{rrrocknrn0113r}

## 1_wanna_b3_a_r0ck5tar (350 points)
### Challenge
I wrote you another song. Put the flag in the picoCTF{} flag format

### Solution
Go read up on the rockstar language. You will realise that the commands `Listen`, `Say` and `If` are unnecessary to the whole code. Remove those, then put it back into the program. Run it, copy the output and convert it to ASCII from Decimal and you will get your flag.

### Flag
picoCTF{BONJOVI}