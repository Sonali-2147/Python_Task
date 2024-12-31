# Python_Task

# Task 1: Reverse a String

## Overview
This task involves reversing a given string without using any built-in string reversal methods. The objective is to implement the functionality manually to demonstrate fundamental programming skills.

## Problem Statement
Write a function to reverse a string without using any built-in functions or methods like `reversed()` or slicing (`[::-1]`).

### Input
- A string, for example: `"hello"`

### Output
- The reversed string, for example: `"olleh"`

## Methodology
To achieve this, we will use the following approach:

1. **Iterative Method**:
   - Create an empty string to store the reversed string.
   - Traverse the input string from the last character to the first.
   - Append each character to the new string.

2. **Algorithm**:
   - Initialize an empty string `reversed_str`.
   - Use a loop to iterate over the string from the last character to the first.
   - Add each character to `reversed_str`.
   - Return `reversed_str` as the output.

### Example
#### Input
```text
"hello"
```
#### Output
```text
"olleh"
```

## Implementation
### Python Code
```python
# Function to reverse a string without using built-in methods
def reverse_string(input_string):
    reversed_str = ""
    for char in range(len(input_string) - 1, -1, -1):
        reversed_str += input_string[char]
    return reversed_str

# Example usage
input_string = "hello"
output_string = reverse_string(input_string)
print(f"Input: {input_string}")
print(f"Output: {output_string}")
```

### Explanation
1. `range(len(input_string) - 1, -1, -1)` creates a sequence from the last index to the first index.
2. Each character at the current index is appended to `reversed_str`.
3. The final reversed string is returned.

## Testing
You can test the function with various inputs to ensure it works correctly:

```python
print(reverse_string("world"))  # Expected output: "dlrow"
print(reverse_string("Python")) # Expected output: "nohtyP"
print(reverse_string("‮12345")) # Expected output: "54321‮"
```

## Edge Cases
1. **Empty String**:
   - Input: `""`
   - Output: `""`
2. **Single Character**:
   - Input: `"a"`
   - Output: `"a"`
3. **Special Characters**:
   - Input: `"@!#"`
   - Output: `"#!@"`

## Conclusion
This task demonstrates how to manually reverse a string by iterating through its characters. It avoids using built-in functions, emphasizing fundamental programming logic.

