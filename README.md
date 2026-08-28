# maximielfrancisco-pixel_Francisco-Maximiel-Anton-V.--PA-1-
------
### 1) Word Rotation Problem - Creates a function that shifts the first letter of a word to the end.
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
------
### 2) Username Builder Problem - Creates a function that converts a first and last name into a lowercase, space-free username
```python
# Define the required function Name
def make_username(first_name, last_name):
    a = first_name.lower().replace(" ", "")
    b = last_name.lower().replace(" ", "")
    return a + "." + b

# It will ask the user to type their first and last name
first = input("Enter first name: ")
last = input("Enter last name: ")

# Call the function with the entered names and display the result
print("Username:", make_username(first, last))

```
##### Step-by-Step Procedure of Functions:
- `first_name.lower().replace(" ", "")` → converts the first name to lowercase and removes all internal spaces.
- `last_name.lower().replace(" ", "")` → converts the last name to lowercase and removes all internal spaces.
- `a + "." + b` → joins the cleaned first name and last name with a period in between.
- `input()` → prompts the user to enter their first name and last name separately.
- `print("Username:", ...)` → calls the function and displays the returned username string.


  Outcome:
```python
A standardized username formatted as firstname.lastname.

Automatically strips out whitespace and enforces lowercase characters.
```

------
### 3) Bookend Swap Problem - Creates a function that swaps the first and last items of a list while keeping the middle items intact
```python
# Define the required function Name
def swap_bookends(items):
    first, *middle, last = items
    return [last] + middle + [first]

# It will ask the user to type items separated by a comma
user_input = input("Enter at least two items (separated by a comma): ").split(",")

# Call the function with the entered items and display the result
print("Resulting list:", swap_bookends(user_input))

```
##### Step-by-Step Procedure of Functions:
- `first, *middle, last = items` → converts the first name to lowercase and removes all internal spaces.
- `[last] + middle + [first]` → converts the last name to lowercase and removes all internal spaces.
- `input(...).split(",")` → takes comma-separated user inputs and splits them into a Python list.
- `print("Resulting list:", ...)` → executes the swap function and displays the reordered list.

  Outcome:
```python
A list where the first and last items switch places.

The original order of all middle elements remains unchanged.
```
