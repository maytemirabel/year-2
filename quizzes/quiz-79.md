# *Quiz 79* #
Create a class that returns the palindromic numbers inside a range A, B inclusive

## Python Code
```.py
def reverse_str(numbers):
    output = []
    for i in range(len(numbers) - 1, -1, -1):
        output.append(numbers[i])
    return "".join(output)

def list_palindromic(a, b):
    palindromic = []
    for num in range(a, b + 1):
        if str(num) == reverse_str(str(num)):
            palindromic.append(num)
    return palindromic

def check_palindromic(unchecked):
    return bool(str(unchecked) == reverse_str(str(unchecked)))

```

## Evidence of Code
<img width="694" alt="Screen Shot 2023-09-30 at 15 34 34" src="https://github.com/maytemirabel/year-2/assets/105724334/11ce04bc-ca8b-4655-85d0-36076f1dddd0">

#### Figure 1: Screenshot displaying code outcome



