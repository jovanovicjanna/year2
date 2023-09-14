# Quiz 074

![Screen Shot 2023-09-13 at 6 23 16](https://github.com/jovanovicjanna/year2/assets/111895127/71f9fb99-643d-41dd-a1bd-5f9893fbe2ce)

## Working on paper

![Screen Shot 2023-09-14 at 20 47 56](https://github.com/jovanovicjanna/year2/assets/111895127/91b5b8d4-3d8c-4f2f-b2e7-a81dc4bcf732)


## Python code

```.py
def bulid_data_pkg(Mac_rx, IP_rx, Mac_sx, IP_sx, data):
    list = []
    final = f"{Mac_rx}|{IP_rx}|{Mac_sx}|{IP_sx}|"
    count = 0
    if len(data) % 4 == 0:
        for i in range(len(data) // 4):
            total = final + f"{data[count:(count + 4)]}"
            list.append(total)
            count += 4
    else:
        for i in range((len(data) // 4) + 1):
            total = final + f"{data[count:(count + 4)]}"
            list.append(total)
            count += 4
    return list

Mac_rx = input("Mac_rx: ")
IP_rx = input("IP_rx: ")
Mac_sx = input("Mac_sx: ")
IP_sx = input("IP_sx: ")
data = input("Data: ")

data_pkgs = bulid_data_pkg(Mac_rx, IP_rx, Mac_sx, IP_sx, data)
print(data_pkgs)
```

## Test

![Screen Shot 2023-09-13 at 6 23 59](https://github.com/jovanovicjanna/year2/assets/111895127/b90aae67-c7de-4506-9ad2-07fb109431a4)
