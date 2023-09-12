
# *Quiz 71* #
Create the code for the IPv6 machine

## Python Code
```.py
from random import randint
addresses = int(input("IPv6 Addresses: "))
# empty list to store the generated IPv6 addresses
list = []
# loop 'addresses' times to generate the specified number of addresses
for a in range(addresses):
    ipv6 = " "
    # 8 segments of the address
    for i in range(8):
        four = " "
        hex = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F"]
        for b in range(4):
            x = randint(0, 14)
            four += hex[x]
            if len(four)==4 and a != 7:
                four += ":" # add a colon as a separator if it's not the last segment
                ipv6 += four
            if len(four)==4 and a == 7:
                ipv6+= four
    list.append(ipv6)
print(list)

```

## Evidence of Code
<img width="1109" alt="Screen Shot 2023-09-12 at 23 34 13" src="https://github.com/maytemirabel/year-2/assets/105724334/16f88679-1e08-40ca-a1e8-3a2a25229b14">

#### Figure 1: Screenshot displaying code outcome
