# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
```
def wrap(string, max_width):
    wrapped_lines = []
    for i in range(0, len(string), max_width):
        wrapped_lines.append(string[i:i+max_width])
    return '\n'.join(wrapped_lines)

text = "This is a sample string that needs to be wrapped after a certain width."
width = 10
result = wrap(text, width)
print(result)

```
## Sample Output

<img width="1270" height="696" alt="444874453-09ca34ae-0056-4fe5-9425-86c07eff5d06" src="https://github.com/user-attachments/assets/7f10b88c-55e4-439f-b6be-8e8d772bb197" />


## Result
Therefore the given Python program has been executed successfully and the output has been verified.
