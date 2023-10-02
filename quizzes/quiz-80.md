# *Quiz 80* #
Create three different programs to calculate the average of a list of numbers 

## Python Code
```.py
# Program #1
def average_with_loop(numbers):
    total = 0
    for number in numbers:
        total += number
    average = total / len(numbers)
    return average

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9]
average = average_with_loop(numbers)
print(average)

# Program #2
def average_with_sum(numbers):
    total = sum(numbers)
    average = total / len(numbers)
    return average

numbers = [11, 22, 33, 44, 55, 66, 77, 88, 99, 101, 111, 121, 131, 141, 151, 161, 171, 181, 191]
average = average_with_sum(numbers)
print(average)

# Program #3
def average_with_while_loop(numbers):
    total = 0
    count = 0
    while count < len(numbers):
        total += numbers[count]
        count += 1
    average = total / len(numbers)
    return average

numbers = [10, 14, 19, 5, 3, 21, 2, 8]
average = average_with_while_loop(numbers)
print(average)

```

## Evidence of Code
<img width="996" alt="Screen Shot 2023-10-02 at 13 59 11" src="https://github.com/maytemirabel/year-2/assets/105724334/abf66da4-472e-4eee-8d65-a9a6d2377907">


#### Figure 1: Screenshot displaying code outcome



