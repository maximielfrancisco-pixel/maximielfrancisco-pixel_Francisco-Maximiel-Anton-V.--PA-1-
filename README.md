# maximielfrancisco-pixel_Francisco-Maximiel-Anton-V.--PA-1-
------
### 1) WORD ROTATION PROBLEM - Creates a function that shifts the first letter of a word to the end.
```python

# Define the required function Name
def rotate_word(text):
    # Code that takes first letter and the other one puts it at the end
    return text[1:] + text[0]

# It will ask the user to type any word
user_word = input("Enter a word: ")

# Call the function with the entered word and display the result
result = rotate_word(user_word)
print("Rotated word:", result)

```
##### Step-by-Step Procedure of Functions:
- `def rotate_word(text)` → defines a function that takes a word string as an input parameter.
- `text[1:]` → slices the string starting from index 1 (the second character) to the end.
- `text[1:] + text[0]` → accesses the first character of the input word.  
- `''.join(sorted(w))` → concatenates the remaining characters with the first character attached at the end.
- `input()` → lets the user type in a word for the program to process.
- `print("Rotated word:", result)` → calls the function and displays the rotated word.

  Outcome:
```python
If the user enters 'Phyton', the program will output:

Rotated word: hytonP
```
