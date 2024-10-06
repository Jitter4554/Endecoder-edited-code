Version : 1.0
Uploaded To Github : 10/3/2024

Created By : @NovaTheTransGirl
Optimized by :@jitter4554 
Lanuage : Python

EXE NOT UPDATED USE THE CODE ITSELF 

This Uses A Reverse Alphabet

Foward Alphabet: 
abcdefghijklmnopqrstuvwxyz1234567890!@#$%^&*()-_=+ :;'/?.>,<[{]}~ABCDEFGHIJKLMNOPQRSTUVWXYZ

Reverse Alphabet:
ZYXWVUTSRQPONMLKJIHGFEDCBA~}]{[<,>.?/';: +=_-)(*&^%$#@!0987654321zyxwvutsrqponmlkjihgfedcba



--------------------------------------------------------------------------------
~~~
Source Code:
import time

def translate():
    alphabet = "abcdefghijklmnopqrstuvwxyz1234567890!@#$%^&*()-_=+ :;'/?.>,<[{]}~ABCDEFGHIJKLMNOPQRSTUVWXYZ
"
    ralphabet = "ZYXWVUTSRQPONMLKJIHGFEDCBA~}]{[<,>.?/';: +=_-)(*&^%$#@!0987654321zyxwvutsrqponmlkjihgfedcba"

    while True:
        choice = input("Encode(1) or Decode(2)? Enter X to Exit: ").strip()

        if choice.lower() == 'x':
            print("Exiting...")
            break

        if choice not in ['1', '2']:
            print("Invalid choice, please try again.")
            continue

        text = input("Input text: ").strip()
        result = ""

        if choice == "1":  # Encoding
            for char in text:
                if char in alphabet:
                    result += ralphabet[alphabet.index(char)]
                else:
                    result += char
            print(f"Encoded Text: {result}")
        
        elif choice == "2":  # Decoding
            for char in text:
                if char in ralphabet:
                    result += alphabet[ralphabet.index(char)]
                else:
                    result += char
            print(f"Decoded Text: {result}")

translate()
~~~~
