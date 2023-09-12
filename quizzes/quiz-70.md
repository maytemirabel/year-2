# *Quiz 70* #
Create the code for the IPv4 machine

## Python Code
```.py
output = input("IPv4 Machine Number: ")
nested for loops to generate and print all possible IPv4 addresses
for a in range(256):
    for b in range(256):
        for c in range(256):
            for d in range(256):
                # print the current combination of (a, b, c, d) as an IPv4 address
                print(f"{a}.{b}.{c}.{d}")
```

## Evidence of Code
<img width="558" alt="Screen Shot 2023-09-12 at 23 28 18" src="https://github.com/maytemirabel/year-2/assets/105724334/ce5577ab-b339-4956-a04c-6bd22da1218f">

#### Figure 1: Screenshot displaying code outcome
