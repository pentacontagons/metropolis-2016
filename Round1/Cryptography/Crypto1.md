#Crypto 1

>Our officers have obtained password dumps storing hacker passwords. After obtaining a few plaintext passwords, it appears that they are all encoded using different number bases.

![](./one.png)

## Problem 1
>0x736e616b65

The Password is in hex, as shown by the 0x prefix. Converting hex to ascii using [this](http://www.rapidtables.com/convert/number/hex-to-ascii.htm)
reveals that the password is `snake`.

## Problem 2
>bWVudGlvbg==

The two equals signs at the end of the password tells us its encrypted with base64. We then convert it to ascii using [this](https://www.base64decode.org/)
which shows that the password is `mention`. 

## Problem 3
> 01110000 01100101 01110010 01110011 01101111 01101110 01100001 01101100 01101100 01111001	

The text looks like its in binary, to we convert it to ascii using [this](http://www.binaryhexconverter.com/binary-to-ascii-text-converter)
to see that the password is `personally`. 

## Problem 4
> 01100001 01000111 00111001 01110101 01100010 00110011 01001010 01101000 01011001 01101101 01111000 01101100	

We try the same strategy as last time, and convert binary to ascii, and get `aG9ub3JhYmxl`, which isn't the password. However
this may also be encrypted, so we try base64 decryption, to get that the password is `honorable`.


