# Cryptography

## Crypto-1 My Best Friend, Julius!
### Challenge
Julius is always sending me cryptic messages. Hmm.

JHLZHY_ZLSSZ_ZLHZOLSSZ_IF_AOL_ZLHZOVYL


### Solution
The name "Julius" gives a hint that it is a Julius Caesar Cipher. Put it into any online decoder to decrypt it. Personally, I prefer Quipquip. The cipher is the traditional Caesar Cipher with a shift of 3

### Flag
CDDC20{CAESAR_SELLS_SEASHELLS_BY_THE_SEASHORE}

## Crypto-2 Cryptic Message
### Challenge
We are not sure what is this gibberish all about, hmm. Can you help us to decode this message?

hq hm kbq jipoox yhnnhatoq qb abkmqjtaq p mijhim bn hknijikaim, ipaS yidikyikq tdbk hqm djIyiaimmbJ pky ipas mhcdoi hk hqmion. hn, pnqij ybhkg mb, bkI mhcdox rkbarm btq poo qsi aikQjpo hknijikaim pky djimikqm bki'm ptyhikai vhqs qsi mqpjqhkg-dbhkq pky qsi abkaoTmhbk, bki cpx dJbytai p mqpjqohKg, qsbtgs dbmmhlox p cijiqjhahbtM, inniaq.

### Solution
Putting the string into quipquip gives us the following text:
```it is not really difficult to construct a series of inferences, eacH dependent upon its prEdecessoR and each simple in itself. if, after doing so, onE simply knocks out all the cenTral inferences and presents one's audience with the starting-point and the conclUsion, one may pRoduce a startliNg, though possibly a meretriciouS, effect.```

By the power of inference, I removed all lowercases letters and only retrieved the capital letters, which gave me "HERETURNS"

### Flag
CDDC20{HERETURNS}

## Crypto-3 Iffy Glyphs
### Challenge
Decrypted text does not include the flag format "CDDC20{}". Add in the flag format "CDDC20{}" during submission, and ensure that the flag string is fully in uppercase, i.e. CDDC20{SAMPLEFLAG}.

MD5("what_is_this.PNG"): 7e50efc4fdaa62b906823f1fee457491

### Solution

Used [this site](https://www.dcode.fr/dancing-men-cipher) to decode the glyphs

### Flag

CDDC20{WELOVETODANCEANDCODEALLDAYLONG}