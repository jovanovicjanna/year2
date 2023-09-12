# Quiz 071

![Screen Shot 2023-09-13 at 0 16 52](https://github.com/jovanovicjanna/year2/assets/111895127/d7e264f8-76f9-4310-aacf-160046a389c7)

## Python code

```.py
def ipv6machine(N: int):
    addresses = []
    for _ in range(N):
        address = []
        for _ in range(8):
            segment = ''.join(rand_int() for _ in range(4))
            address.append(segment)
        addresses.append(':'.join(address))
    return addresses

N = 5
generated_addresses = ipv6machine(N)
for address in generated_addresses:
    print(address)
```

## Test
![Screen Shot 2023-09-13 at 0 18 00](https://github.com/jovanovicjanna/year2/assets/111895127/48c9fdd2-a70c-490b-a6fc-91f95458a082)
