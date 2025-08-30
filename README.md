# PA-1-DE-BORJA
(REUPLOADED)

# Python Mini Projects 

This repository contains three Python exercises that demonstrate basic programming concepts.

## Projects

- **Alphabet Soup**  
I created a function [alphabet_soup] which;
  1. Accepts a string (word) from the user as input.
  2. Utilizes Python’s built-in `sorted()` function to arrange the characters in alphabetical order.
  3. Joins the sorted characters back together using `"".join()`.
  4. Prints the final arranged word.  

- **Emotify**  
By utilizing the dictionary (emoticons) created;
  1. Sentence from user input is split into Individual wordsusing `.split()`.
  2. Each word is checked to see if it matches any existing keys in the dictionary.
  3. It is then replaced/converted with the emoticon. Otherwise, the original word is kept.
  4. The list of words was joined back and displayed with  return " ".join(result).

- **Unpack List**
  1. Python’s unpacking feature is utilized:
  - `first` stores the first element.
  - `last` stores the last element.
  - `*middle` captures all the elements in between as a list.
  2. The program takes user input of numbers separated by spaces.
  3. The input string is then converted into a list with `.split()`.
  4. The unpacked parts (first, middle, last) are then printed.  
