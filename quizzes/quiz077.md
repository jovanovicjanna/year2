# Quiz 077

![Screen Shot 2023-09-13 at 6 41 13](https://github.com/jovanovicjanna/year2/assets/111895127/6df64335-ca82-4200-884a-af24737cccb3)

## Python code

```.py
def parity_check(data):
    first_digit = int(data[0])
    total_sum = 0

    for i in range(1, len(data)):
        total_sum += int(data[i])

    if total_sum % 2 == 0 and first_digit == 1:
        has_error = False
    elif total_sum % 2 == 1 and first_digit == 0:
        has_error = False
    else:
        has_error = True

    return has_error

test1 = parity_check("100111001011001110010110011100101")
print(test1)

test2 = parity_check("011101111101110111110111001111")
print(test2)
```

## Test
![Screen Shot 2023-09-13 at 6 47 32](https://github.com/jovanovicjanna/year2/assets/111895127/cc59c2b0-6f62-461f-a0bb-7004af980e8d)
