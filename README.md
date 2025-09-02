# PA-1-DE-BORJA

Problem #1
- **Alphabet Soup**

```
def alphabet_soup(word: str):
    return ''.join(sorted(word))

word = input("Enter ANYTHING!: ")
print("Alphabet SOUP:", alphabet_soup(word))
Alphabet SOUP:    STUaaefiimnnooorssttvy
```

I created a function [alphabet_soup] which;
  1. Accepts a string (word) from the user as input.
  2. Utilizes Python’s built-in `sorted()` function to arrange the characters in alphabetical order.
  3. Joins the sorted characters back together using `"".join()`.
  4. Prints the final arranged word.  

Problem #2
- **Emotify**

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
```

By utilizing the dictionary created (emoticons);
  1. Sentence from user input is split into Individual words using `.split()`.
  2. Each word is checked to see if it matches any existing keys in the dictionary.
  3. It is then replaced/converted with the emoticon. Otherwise, the original word is kept.
  4. The list of words was joined back and displayed with  return " ".join(result).

Problem #3
- **Unpack List**

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

  1. Python’s unpacking feature is utilized:
  - `first` stores the first element.
  - `last` stores the last element.
  - `*middle` captures all the elements in between as a list.
  2. The program takes user input of numbers separated by spaces.
  3. The input string is then converted into a list with `.split()`.
  4. The unpacked parts (first, middle, last) are then printed.  
