# Challenge 2 - JavaSubstitution
> It is time for more ciphers!

## The Challenge
For this challenge, you will need to solve a substitution cipher. There are no files to read. Instead you will be given two Strings: an output and a key. The key is the cipher alphabet you will need to use to decode the output.

Here is the String:
```java
String output = "ugs ignl vgok ugfgk qgk muwl eafv a iav?";
```
And here is the key:
```java
String key = "NQhmgUXvfIWRosBkZclAejDtyp";
```
Notice that there ARE uppercase letter in the key. This key isn't correct yet. To fix it, you will need to sort the letters by ASCII value (using whatever sorting algorithm you wish). After doing this, you can convert the letters all to lowercase, and then use it as your key.

After finding the correct key, you can then decode the output string.

## Rules
1. Your code should be able to decode any string encoded with the proper key
2. All sorting algorithms are allowed (but you should try something new)
## Cheat sheet
### Array things in Java
```java
int[] arr = new int[]{1, 2, 3, 4, 5};

//prints all values in arr
for(int i = 0; i < arr.length; i++){
	System.out.println(arr[i]);
}
```
### String things in Java
```java
String s = "abcdefg";
System.out.print(s.charAt(0)); //prints 'a'
System.out.print(s.charAt(6)); //prints 'g'
System.out.print(s.charAt(7)); //throws an error
```
### Conversion things in Java
```java
//converting a character to an integer
char c = 'a';
int intOfC = (int) c;

//converting an integer to a character
int i = 5;
char charOfI = (char) i;
```
