# Quiz 073

![Screen Shot 2023-09-13 at 0 45 43](https://github.com/jovanovicjanna/year2/assets/111895127/aaa81f85-8386-44b1-bd71-8778b3612e3d)

## Python code

```.py
import random
def check_mac(mac):
    return len(mac) == 17 and mac.count(":") == 5

def generate_ipv4():
    ipv4 = ".".join(str(random.randint(0, 255)) for a in range(4))
    return ipv4

def update(table, mac):
    if check_mac(mac):
        if mac in table:
            return table[mac]
        else:
            while True:
                ip = generate_ipv4()
                if ip not in table.values():
                    table[mac] = ip
                    return ip

def display(table):
    print("Routing Table:")
    for mac, ip in table.items():
        print(f"MAC: {mac}, IP: {ip}")

table = {}
while True:
    mac_address = input("Enter MAC address: ")
    ip_address = update(table, mac_address)
    display(table)
```

## Test
![Screen Shot 2023-09-13 at 0 46 53](https://github.com/jovanovicjanna/year2/assets/111895127/923fc2ef-f95e-4946-858d-dd2f4c7b8b10)


