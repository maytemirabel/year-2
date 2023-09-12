# *Quiz 70* #
Create the code for the IPv4 machine

## Python Code
```.py
def generate_ipv4_addresses():
    output = input("IPv4 Machine Number: ")

    # nested for loops to generate and print all addresses
    for a in range(256):
        for b in range(256):
            for c in range(256):
                for d in range(256):
                    # print the combination of (a, b, c, d) as an IPv4 address
                    print(f"{a}.{b}.{c}.{d}")
generate_ipv4_addresses()

```

## Evidence of Code
<img width="878" alt="Screen Shot 2023-09-13 at 0 12 51" src="https://github.com/maytemirabel/year-2/assets/105724334/ef403282-d366-43b3-86f2-a3f743ca72d9">

#### Figure 1: Screenshot displaying code outcome
