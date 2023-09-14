# Quiz 075

![Screen Shot 2023-09-13 at 6 25 14](https://github.com/jovanovicjanna/year2/assets/111895127/77c5ee88-15fd-4a72-b14c-750f00361b17)

## Working on paper
![Screen Shot 2023-09-14 at 20 34 05](https://github.com/jovanovicjanna/year2/assets/111895127/a556a9ee-3caf-48bf-8413-68af68c48a63)


## Python code

```.py
def convert(data_str):
    binary_str = ""
    for char in data_str:
        binary_char = ''
        char_code = ord(char)
        while char_code > 0:
            remainder = char_code % 2
            binary_char = str(remainder) + binary_char
            char_code = char_code // 2
        while len(binary_char) < 8:
            binary_char = '0' * (8 - len(binary_char)) + binary_char
        binary_str += f"{binary_char} "
    return binary_str.strip()

test1 = convert("Hello world!")
print(test1)

test2 = convert("42 is the answer.")
print(test2)

test3 = convert("ABC123")
print(test3)
```

## Test

![Screen Shot 2023-09-13 at 6 32 02](https://github.com/jovanovicjanna/year2/assets/111895127/4848181b-880b-46de-8b52-eaaf8e657f94)
