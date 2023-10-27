# *Quiz 84* #

## Python Code
```.py
class Citizen:
    def __init__(self, name, city, status):
        self.name = name
        self.city = city
        self.status = status

    def getName(self):
        return self.name
    def getCity(self):
        return self.city
    def getStatus(self):
        return self.status

class Employee(Citizen):
    def __init__(self, name, city, status, salary):
        self.annual_salary = salary
        Citizen.__init__(self, name, city, status)

    def getSalary(self):
        return self.annual_salary

class PartTimeEmployee:
    def __init__(self, name, city, status, salary, fraction, member):
        self.time_fraction = fraction
        self.union_member = member
        Citizen.__init__(self, name, city, status)
        Employee.__init__(self, name, city, status, salary)

    def getFraction(self):
        return self.time_fraction
    def getMember(self):
        return self.union_member

citizen = Citizen("bob", "kyoto", "alive")
employee = Employee("cathy", "tokyo", "alive", 50000)
part_time_employee = PartTimeEmployee("tim", "karuizawa", "alive", 25000, 0.5, True)

print(citizen.getName(), citizen.getCity(), citizen.getStatus())
print(employee.getName(), employee.getSalary())
print(part_time_employee.getMember(), part_time_employee.getFraction())

```

## Evidence of Code

<img width="779" alt="Screen Shot 2023-10-27 at 13 28 07" src="https://github.com/maytemirabel/year-2/assets/105724334/09b35a15-f941-47ae-90dd-c9d88fed7fcb">



#### Figure 1: Screenshot displaying code outcome



