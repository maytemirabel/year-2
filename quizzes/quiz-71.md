
# *Quiz 71* #
Create the code for the IPv6 machine

## Python Code
```.py
from random import randint
def generate_ipv6_addresses(num_addresses):
    # empty list to store the generated IPv6 addresses
    ipv6_list = []
    # loop 'num_addresses' times to generate the specified number of addresses
    for _ in range(num_addresses):
        ipv6 = ""
        # generate 8 segments of the IPv6 address
        for _ in range(8):
            four = ""
            hex_chars = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F"]
            for _ in range(4):
                x = randint(0, 15)
                four += hex_chars[x]
            # add a colon as a separator if it's not the last segment
            if len(ipv6) > 0:
                ipv6 += ":"
            ipv6 += four
        ipv6_list.append(ipv6)
    return ipv6_list
addresses = int(input("IPv6 Addresses: "))
result = generate_ipv6_addresses(addresses)
print(result)
```

## Evidence of Code
<img width="1080" alt="Screen Shot 2023-09-13 at 0 16 07" src="https://github.com/maytemirabel/year-2/assets/105724334/d6b9f209-1b83-417e-9cd9-08c512cbdc4b">


#### Figure 1: Screenshot displaying code outcome
