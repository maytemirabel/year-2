# *Quiz 76* #
The physical layer is also in charge of detecting and trying to correct errors in the data transmitted. One simple way would be to send copies of the data and check that the copies match. Assume the data is 2 copies of the data plus original.


## Python Code
```.py
def check_data_for_error(data):
    error = ""
    x = len(data)
    y = data[0:x // 3]
    z = data[x // 3:(x * 2) // 3]
    w = data[(2 * x) // 3: -1]

    # check if any parts are equal or if all parts are equal
    if y == z or y == w or z == w or (y == z and y == w):
        error = False
    else:
        error = True

    return error
data = input("Data: ")
result = check_data_for_error(data)
print(result)

```

## Evidence of Code

<img width="1082" alt="Screen Shot 2023-09-13 at 0 10 16" src="https://github.com/maytemirabel/year-2/assets/105724334/99932315-5b00-4eac-80e4-7a8208d13f81">

#### Figure 1: Screenshot displaying code outcome


