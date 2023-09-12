# *Quiz 77* #
The physical layer is also in charge of detecting and trying to correct errors in the data transmitted. Create a function to check the parity bit of a data string, and determine if there is an error. Assume parity=1 for an even number of ones

## Python Code
```.py
def check_data_for_error(data):
    # assuming no error initially
    error = False
    x = int(data[0])
    count = 0

    # loop through the characters in input (excluding the first character)
    for i in range(1, len(data)):
        count += int(data[i])
    if count % 2 == 0 and x == 1:
        error = False
    elif count % 2 == 1 and x == 0:
        error = False
    else:
        error = True
    return error

data = input("Data: ")
result = check_data_for_error(data)
print(result)
```

## Evidence of Code
<img width="1106" alt="Screen Shot 2023-09-13 at 0 07 29" src="https://github.com/maytemirabel/year-2/assets/105724334/a7cdb47d-35d8-4a7e-beaa-7ae458aed435">


#### Figure 1: Screenshot displaying code outcome


