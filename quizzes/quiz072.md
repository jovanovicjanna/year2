# Quiz 072

![Screen Shot 2023-09-13 at 0 21 14](https://github.com/jovanovicjanna/year2/assets/111895127/b4f26867-1e1b-4ccc-a384-e8adb7cb4267)

## Python code
```.py

def rand_int():
    rand_index = random.randint(0, 15)
    hex_digits = ['0','1','2','3','4','5','6','7','8','9','A','B','C','D','E','F']
    n = hex_digits[rand_index]
    return n

def macGenerator(N:int):
    addresses = []
    for _ in range(N):
        address = []
        for _ in range(6):
            segment = ''.join(rand_int() for _ in range(2))
            address.append(segment)
        addresses.append(':'.join(address))
    return addresses

N = 5
generated_addresses = macGenerator(N)
for address in generated_addresses:
    print(address)
```

## Test

![Screen Shot 2023-09-13 at 0 22 08](https://github.com/jovanovicjanna/year2/assets/111895127/4cbcc32a-078a-49f3-80af-1f0a65a5fc23)
