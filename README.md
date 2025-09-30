# PA-1-DE-BORJA

This Python script contains three mini-problems designed to practice basic string manipulation, dictionaries, and list unpacking.

---

## Problem #1: Alphabet Soup

The function `alphabet_soup()`:
1. Accepts a string from the user via `input()`.
2. Uses Python’s built-in `sorted()` function to sort the characters in alphabetical order.
3. Joins the sorted characters using `"".join()` to form a new string.
4. Prints the result as "Alphabet SOUP".

```
def alphabet_soup(word: str):
    return ''.join(sorted(word))

word = input("Enter ANYTHING!: ")
print("Alphabet SOUP:", alphabet_soup(word))

```

## Problem #2: Emotify

The function `emotify()`:
1. Defines a dictionary of common emotion words mapped to emoticons.
2. Splits the input sentence into individual words using `.split()`.
3. Checks each word (case-insensitive) against the dictionary.
4. Replaces matching words with their emoticons.
5. Joins and returns the modified sentence.

```
def emotify(sentence):
    emoticons = { "smile": ":)", "grin": ":D", "sad": ":((", "mad": ">:("}
    words = sentence.split()
    result = []
    
    for word in words:
        if word.lower() in emoticons:
            result.append(emoticons[word.lower()])
        else:
            result.append(word)
    
    return " ".join(result)

sentence = input("Enter a sentence: ")
print("Converted:", emotify(sentence))
```

## Problem #3: Unpack List

The function `unpack_list()`:
1. Uses the unpacking syntax `first, *middle, last` to divide a list into:
   - `first`: the first item
   - `middle`: all items in between (as a list)
   - `last`: the last item
2. Input is collected as a space-separated string and converted into a list with `.split()`.
3. The three parts are printed.

```
def unpack_list(lst):
    first, *middle, last = lst
    print("first:", first)
    print("middle:", middle)
    print("last:", last)

user = input("Enter numbers separated by spaces: ")
lst = user.split()
unpack_list(lst)
```

---VERSION 2---
