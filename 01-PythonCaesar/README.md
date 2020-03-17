# Challenge 1 - PythonCaesar
> Friends, Romans, Pythonistas! Lend me your code!

## The Challenge
In this folder, there is a text file called `encoded.txt` encoded with the caesar cipher with a shift of 13. The character set used is:
```python
charSet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm',
           'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
           ',', '.', '!', '?']
```
Note that there are no uppercase letters. If you're unfamiliar with the Caesar Cipher, [check out the Wikipedia article](https://en.wikipedia.org/wiki/Caesar_cipher).

Your job is to make a Python file called `caesar.py` that has the following function:
```python
def decode_file(filename, shift):
    ...
```
that takes in the name of a file to decode (a string) and the number of characters to shift by (an integer) and prints the result to the screen.

## Rules
1. No modules are allowed outside of the standard library. If you have to `pip install` something, you're doing it wrong.
2. Your function should work on any file you give it, with any shift you give it - not just `encoded.txt` with a shift of 13.
3. If your function encounters a character in the file that's not in it's character set (#, for example), it should just skip over it. This means you have to learn `try:` and `except` in Python.
4. The file passed WILL have multiple lines. You are to decode it line by line (see cheat sheet below for how to read in a file line by line).

## Cheat sheet
### File reading in Python:
```python
with open(file_name, "r") as file:
    for line in file:
        print(line)
```
### List things in Python
```python
ls = ['first_thing', 'second_thing', 'third_thing', 'fourth_thing']
print(ls[0])               # first_thing
print(ls[1])               # second_thing
print(ls[:2])              # [first_thing, second_thing]
print(ls[1:3])             # [second_thing, third_thing]
print('first_thing' in ls) # True
print('fifth_thing' in ls) # False
```
### String things in Python
```python
string = "abcdefg"
print(string[0])   # a
print(string[1])   # b
print(string[-1])  # g
print(string[:3])  # abc
print(string[1:4]) # bc
```
