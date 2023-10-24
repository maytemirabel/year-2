# *Quiz 84* #

## Python Code
```.py
class FourDigitNumber:
    def __init__(self, value):
        self.intvalue = value
        self.thousandigit = value // 1000
        self.hundreddigit = (value // 100) % 10
        self.tensdigit = (value // 10) % 10
        self.onesdigit = value % 10

    def assign(self):
        return f"int value: {self.intvalue}, thousand digit: {self.thousandigit}, hundred digit: {self.hundreddigit}, tens digit: {self.tensdigit}, ones digit: {self.onesdigit}"

test = FourDigitNumber(1234)
print(test.assign())

```

## Evidence of Code
<img width="1113" alt="Screen Shot 2023-10-24 at 18 44 12" src="https://github.com/maytemirabel/year-2/assets/105724334/0df01ead-e32e-422b-bc84-9452c8b4203a">

#### Figure 1: Screenshot displaying code outcome


