# Crytography

## Things you need

## Challenges
- The Numbers

## The Numbers (50 points)
### Challenge
The numbers... what do they mean?

### Solution
Upon looking at the image, the numbers given look like the flag. The first 7 numbers coincidentally look like "picoCTF", and the curly brackets contain what could be the flag. It doesn't take much time to realise that these numbers are the positions of the alphabets in the alphabetical series. Where P is 16 and I is 9 for example. Just match each number to their corresponding letter, and you will get the flag. You can use a script for this too.

### Flag
PICOCTF{THENUMBERSMASON}

## 13 (100 points)
### Challenge
Cryptography can be easy, do you know what ROT13 is? cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}

### Solution
ROT13 is an encryption algorithm. Look for a rot13 decoder online and put in the text given above.

### Flag
picoCTF{not_too_bad_of_a_problem}

## Easy1 (100 points)
### Challenge
The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help UFJKXQZQUNB with the key of SOLVECRYPTO. Can you use this table to solve it?.

### Solution
Just use the table they provide to match each letter from the key and the text in order to get the plaintext. Another way is to put it into a Vigenere Cipher decoder and obtain the flag.

### Flag
picoCTF{CRYPTOISFUN}

## Caesar (100 points)
### Challenge
Decrypt this message. You can find the ciphertext in /problems/caesar_5_d706b250ed3c6d2d2c72155de301a2f1 on the shell server.

### Solution
The name kind of already gives it away. It is probably a Caesar Cipher challenge. cd to the directory above in order to get the encrypted flag. You will notice that "picoCTF" is not encrypted. Put only the contents of the curly brackets into a Caesar Cipher decoder with a shift value of 3 and obtain the flag. 

### Flag
picoCTF{crossingtherubiconapisvsuj}

## Flags (200 points)
### Challenge
What do the flags mean?

### Solution
Upon opening the image, we can realise that the flag is encoded using the maritime flag system. Look for an online navy signal decoder and put in the images in the correct sequence to get the flag.

### Flag
PICOCTF{F1AG5AND5TUFF}

## Mr WorldWide (200 points)
### Challenge
A musician left us a message. What's it mean?

### Solution
Upon looking at the txt file given, it looks like many coordinates placed into the flag. It's a good guess to say each letter is the first letter of the location name of each coordinate. For example, the first set of coordinates "(35.028309, 135.753082)" point to Kamigyo, so we take the "K" from it. Repeat this for the other coordinates

### Flag
picoCTF{KODIAK_ALASKA}

## Tapping (200 points)
### Challenge
Theres tapping coming in from the wires. What's it saying nc 2019shell1.picoctf.com 49914.

### Solution
Upon netcat-ting, you get a string of dots and dashes. This looks a lot like morse code, so I looked for a morse code decoder and input that chunk inside. Press decode and you get your flag.

### Flag
PICOCTF{M0RS3C0D31SFUN903140448}

## la cifra de (200 points)
### Challenge
I found this cipher in an old book. Can you figure out what it says? Connect with nc 2019shell1.picoctf.com 39776.

### Solution
When I got the text, I just threw it into every cipher I could think of, starting with Caesar just to experiment. Finally, I used https://www.guballa.de/vigenere-solver to brute force the cipher, on the assumption it was a Vigenere Cipher. I managed to get a clear text with the key "flag" and got this:
```
It is interesting how in history people often receive credit for things they did not create

During the course of history, the Vigenère Cipher has been reinvented many times

It was falsely attributed to Blaise de Vigenère as it was originally described in 1553 by Giovan Battista Bellaso in his book La cifra del. Sig. Giovan Battista Bellaso 

For the implementation of this cipher a table is formed by sliding the lower half of an ordinary alphabet for an apparently random number of places with respect to the upper half *picoCTF{b311a50_0r_v1gn3r3_c1ph3r1119c336}*

The first well-documented description of a polyalphabetic cipher however, was made around 1467 by Leon Battista Alberti.

The Vigenère Cipher is therefore sometimes called the Alberti Disc or Alberti Cipher.

In 1508, Johannes Trithemius invented the so-called tabula recta (a matrix of shifted alphabets) that would later be a critical component of the Vigenère Cipher.

Bellaso’s second booklet appeared in 1555 as a continuation of the first. The lower halves of the alphabets are now shifted regularly, but the alphabets and the index letters are mixed by means of a mnemonic key phrase, which can be different with each correspondent.
```
### Flag
picoCTF{b311a50_0r_v1gn3r3_c1ph3r1119c336}

## rsa-pop-quiz (200 points)
### Challenge
Class, take your seats! It's PRIME-time for a quiz... nc 2019shell1.picoctf.com 2611

### Solution
Using Netcat will give you a series of calculation challenges from RSA to solve. After you solve 7 of them you will get the flag.

### Flag
picoCTF{wA8_th4t$_ill3aGal..o1c355060}

## 
### Challenge


### Solution


### Flag
