# *Quiz 75* #
The physical layer of the OSI model primarily deals with the physical aspects of data transmission, including the hardware, transmission medium (cable, waves, etc.), encoding, signaling, and synchronization necessary to send raw bits between devices. Create a function that converts the input: str to a binary: str


## Python Code
```.py
def convert(message: str):
    product = ""
    # loop through each character in message
    for i in message:
        binary = ''
        n = ord(i)  # get ASCII value
        # convert ASCII to binary
        while n > 0:
            res = n % 2
            binary = str(res) + binary
            n = n // 2
        while len(binary) < 8:
            binary = '0' * (8 - len(binary)) + binary
        product += f"{binary} "
    return product.strip()

message = "Hello!"
result = convert(message)
print(result)

```

## Evidence of Code
<img width="1114" alt="Screen Shot 2023-09-13 at 2 50 37" src="https://github.com/maytemirabel/year-2/assets/105724334/e3a122f5-36e5-49bb-a0da-fb1d617c6629">

#### Figure 1: Screenshot displaying code outcome
