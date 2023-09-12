
# *Quiz 73* #
Create a simple program to manage a network routing table.

## Python Code
```.py
from random import randint
# check if MAC address is in the correct format
def check_mac(mac: str) -> bool:
    return len(mac) == 17 and mac.count(":") == 5

# generate a random IPv6 address
def IPv6():
    ipv6 = ""
    for a in range(8):
        four = ""
        hex = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F"]
        for b in range(4):
            x = randint(0, 14)
            four += hex[x]
            if len(four) == 4 and a != 7:
                four += ":"
                ipv6 += four
            if len(four) == 4 and a == 7:
                ipv6 += four
    return ipv6

#get or generate an IPv6 address based on the MAC address
def get_ipv6_address(mac: str) -> str:
    routing_table = {}
    if check_mac(mac):
        if mac in routing_table:
            return routing_table[mac]
        else:
            while True:
                ipv6 = IPv6()
                if ipv6 not in routing_table.values():
                    routing_table[mac] = ipv6
                    return ipv6
mac_address = "00:1A:2B:3C:4D:5E"
ipv6_address = get_ipv6_address(mac_address)
print(f"IPv6 Address for MAC {mac_address}: {ipv6_address}")


```

## Evidence of Code

<img width="1080" alt="Screen Shot 2023-09-13 at 3 35 33" src="https://github.com/maytemirabel/year-2/assets/105724334/648e0ee2-1e41-4975-9605-9d21afedba27">


#### Figure 1: Screenshot displaying code outcome
