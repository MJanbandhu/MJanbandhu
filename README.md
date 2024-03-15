```python
def rotate_alphabet(text, shift):
    result = ""
    for char in text:
        if char.isalpha():
            ascii_offset = 65 if char.isupper() else 97
            shifted = (ord(char) - ascii_offset + shift) % 26 + ascii_offset
            result += chr(shifted)
        else:
            result += char
    return result

def print_rotated_text():
    name = "Mohit Janbandhu"
    shifted_name = rotate_alphabet(name, 1)  # Rotate each alphabet by 1
    print(shifted_name)

    title = "Certified Data Scientist"
    shifted_title = rotate_alphabet(title, 3)  # Shift title by 3
    print(shifted_title)

print_rotated_text()
```
Npiju Kbocboeiv
Fhuwlilhg Gdwd Vflhqwlvw
