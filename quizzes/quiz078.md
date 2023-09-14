# Quiz 078

![Screen Shot 2023-09-14 at 17 37 37](https://github.com/jovanovicjanna/year2/assets/111895127/f3a0dfc7-10d2-43ea-bfcf-97f1bbbac6be)

## Working on paper
![Screen Shot 2023-09-14 at 20 44 31](https://github.com/jovanovicjanna/year2/assets/111895127/093734f9-5b04-4ef9-b7f6-a4e4573fc608)

## Python code
```.py
def firewall(data):
    if len(data) < 16:
        return  ""

    bits = data[:16]
    num = int(bits, 2)

    if num == 80 or num == 22123:
        return "Allowed", data[16:]
    else:
        return "Filtered", ""

test1 = firewall("100111001011001110010110011100101")
print(test1)

test2 = firewall("010101100110101111110111001111")
print(test2)
```
## Test
![Screen Shot 2023-09-14 at 17 40 06](https://github.com/jovanovicjanna/year2/assets/111895127/965fc59a-3b31-4e53-8d3f-67c8c3705a66)
