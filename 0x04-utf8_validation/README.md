# 0x04. UTF-8 Validation

Mahbub Mohammed Kingosway@gmail.com Da-Rumi

## 🧠 Objective

Implement a method that checks whether a given data set represents a valid UTF-8 encoding.

## 📝 Requirements

- Function Prototype:
  def validUTF8(data)
- Returns:
  - True if data is a valid UTF-8 encoding
  - False otherwise
- A character in UTF-8 can be 1 to 4 bytes long
- The input data may represent multiple characters
- Each item in data is an integer (representing one byte), and only the 8 least significant bits are relevant

## 💻 Example Usage

#!/usr/bin/python3
"""
Main file for testing
"""

validUTF8 = __import__('0-validate_utf8').validUTF8

data = [65]
print(validUTF8(data))  # True

data = [80, 121, 116, 104, 111, 110, 32, 105, 115, 32, 99, 111, 111, 108, 33]
print(validUTF8(data))  # True

data = [229, 65, 127, 256]
print(validUTF8(data))  # False

### Sample Output:
True
True
False

## 📚 Resources

- UTF-8 on Wikipedia: https://en.wikipedia.org/wiki/UTF-8
- What is UTF-8? (YouTube): https://www.youtube.com/watch?v=MijmeoH9LT4

