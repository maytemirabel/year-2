# *Quiz 74* #
A data package is built by splitting the data into fixed sizes (load) and attaching a header that contains the MAC address, the IP address of the sender (sx) and destination (rx), and a sequence number to reconstruct the data. Create the function below
## Python Code
```.py
def create_packages():
    macrx = input("macrx: ")
    IP_rx = input("IP_rx: ")
    mac_sx = input("mac_sx: ")
    IP_sx = input("IP_sx: ")
    data = input("data: ")

    list_pkg = []
    header = f"{macrx}|{IP_rx}|{mac_sx}|{IP_sx}|"
    count = 0
    # check if length is divisible by 4
    if len(data) % 4 == 0:
        # loop to split data into 4 parts
        for i in range(len(data) // 4):
            total = header + f"{data[count:(count+4)]}"
            list_pkg.append(total)
            count += 4
    else:
        for i in range((len(data) // 4) + 1):
            total = header + f"{data[count:(count + 4)]}"
            list_pkg.append(total)
            count += 4
    return list_pkg
result = create_packages()
print(result)


```

## Evidence of Code

<img width="1255" alt="Screen Shot 2023-09-13 at 2 58 52" src="https://github.com/maytemirabel/year-2/assets/105724334/44665188-f386-4396-86d6-2c8bbd42dfd8">


#### Figure 1: Screenshot displaying code outcome
