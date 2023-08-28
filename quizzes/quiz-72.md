# *Quiz 72* #
Create the code for the Mac generator machine

## Python Code
```.py
import random
def macGenerator(N:int):
    hex_digits = "0123456789ABCDEF"
    output = []

    for address in range(N):
        mac = ""
        for groups in range(6):
            group = ""
            for digits in range(2):
                group += random.choice(hex_digits)
            mac += group + ":"
        output.append(mac[:-1])

    return output
```

## Evidence of Code
<img width="1187" alt="Screen Shot 2023-08-28 at 12 11 30" src="https://github.com/maytemirabel/year-2/assets/105724334/a84d6259-712e-4165-ab70-7088da0d53c3">=
#### Figure 1: Screenshot displaying code outcome
