# *Quiz 78* #

## Python Code
```.py
def layer4_firewall(data):
    x = data[:16]
    num = 0
    output = ""
    msg = ""
    for i in range(16):
        num += int(x[i]) * (2 ** (15 - i))

    if num == 22123 or num == 80:
        output = "Allowed"
        msg = data[16:]
    else:
        output = "Filtered"
        msg = None

    return output, msg

```

## Evidence of Code
<img width="1083" alt="Screen Shot 2023-09-13 at 20 35 41" src="https://github.com/maytemirabel/year-2/assets/105724334/d7e36fef-a7f9-4197-9c25-130b45b7c8f3">

#### Figure 1: Screenshot displaying code outcome



