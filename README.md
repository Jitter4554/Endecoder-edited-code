Version : 1.0
Uploaded To Github : 10/3/2024

Created By : @NovaTheTransGirl
Lanuage : Python

This Uses A Reverse Alphabet

Foward Alphabet: 
abcdefghijklmnopqrstuvwxyz1234567890!@#$%^&*()-_=+ :;'/?.>,<[{]}~ABCDEFGHIJKLMNOPQRSTUVWXYZ

Reverse Alphabet:
ZYXWVUTSRQPONMLKJIHGFEDCBA~}]{[<,>.?/';: +=_-)(*&^%$#@!0987654321zyxwvutsrqponmlkjihgfedcba



--------------------------------------------------------------------------------

Source Code:
```
import time

a = input("Encode(1) or Decoded(2)? : ")

alphabet = "abcdefghijklmnopqrstuvwxyz1234567890!@#$%^&*()-_=+ :;'/?.>,<[{]}~ABCDEFGHIJKLMNOPQRSTUVWXYZ"
ralphabet = "ZYXWVUTSRQPONMLKJIHGFEDCBA~}]{[<,>.?/';: +=_-)(*&^%$#@!0987654321zyxwvutsrqponmlkjihgfedcba"
f = ""
if a == "1":
    b = input("Input Text To be Encode! : ")

    c = len(b)
    for x in range(0, c):
        d = alphabet.index(b[x])

        f = f + ralphabet[d]

    print(f)
else:
    b = input("Input Decoded Text! : ")

    c = len(b)
    for x in range(0, c):
        d = ralphabet.index(b[x])

        f = f + alphabet[d]

    print(f)


z=input("[X] to call close : ")
if z == "X":
    exit()

if z == "x":
    exit()```
