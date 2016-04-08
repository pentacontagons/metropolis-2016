# Crypto 5

> Our officers have obtained password dumps storing hacker passwords. After obtaining a few plaintext passwords, it appears that some sort of transposition cipher was used.

![](./five.jpg)

## Problem 1

> WOMCIWD IKMOZ5IHU UI,LF OL EAMSAE ER-AW84TTS EUB T.TJ-5	

From the description, we get that its a transpostition cipher. We find that there are two common types of transposition ciphers, 
columnar transposition and rail fence ciphers. We try transposition ciphers with [this](http://tholman.com/other/transposition/), trying 
different small key lengths, but we only get garbage.

Next, we try the rail cipher on [this](http://www.geocachingtoolbox.com/index.php?page=railFenceCipher), and get a message with 3 rails. 
As a result, we get the message `WITHOUT MUSIC, LIFE WOULD BE A MISTAKE. METRO-JAZW-8545`, so the password is `METRO-JAZW-8545`.

## Problem 2

> Y CHWSH.A8OTB HTA I ETED -Z5USEEA TUSOE  LMOW4 U HNE OHT NWRERV5MTGY IOT-

We try the rail cipher as before, and brute force the number of rails, getting that it is `YOU MUST BE THE CHANGE THAT YOU WISH TO SEE IN THE WORLD. METRO-AZWV-5458`,
so the password is `METRO-AZWV-5458`
