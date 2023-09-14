# Quiz 076

![Screen Shot 2023-09-13 at 6 33 30](https://github.com/jovanovicjanna/year2/assets/111895127/d0124d64-e5e9-4a6b-bc24-f17c26dfb1ed)

## Working on paper
![Screen Shot 2023-09-14 at 20 38 05](https://github.com/jovanovicjanna/year2/assets/111895127/40c7f5ca-c564-4aa6-b4ad-c6096cc06d42)


## Python code
```.py
def check_error(data):
    data_len = len(data)
    part1 = data[0:data_len // 3]
    part2 = data[data_len // 3:(data_len * 2) // 3]
    part3 = data[(2 * data_len) // 3:]

    if part1 == part2 == part3:
        has_error = False
    else:
        has_error = True

    return has_error

test1 = check_error("100111001011001110010110011100101")
print(test1)
test2 = check_error("011101111101110111110111001111")
print(test2)
```
## Test

![Screen Shot 2023-09-13 at 6 40 23](https://github.com/jovanovicjanna/year2/assets/111895127/2b2a8c71-3a84-4706-ac45-c0b14efee42b)
