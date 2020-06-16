# General Skills
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