# *Quiz 69*
One array holds the daily sales of a clothing store in no particular order. You are tasked with finding the profit of the best day in comparison to the worst day. That is, how much more was sold in Japanese Yens on the best day?

## Data set
<img width="317" alt="Screen Shot 2023-08-22 at 20 33 15" src="https://github.com/maytemirabel/Unit-3/assets/105724334/c40eeb41-8598-4513-9b0b-8a1f50ffc318">

#### Figure 1: Array displaying the sales made on a particular day

## Python Code
```.py
daily_sales = [100, 45, 12, 3, 56, 7]

# initialize variables for best and worst sales
best_sales = daily_sales[0]
worst_sales = daily_sales[0]

# finding the best and worst sales
for sales in daily_sales:
    # loop checking if the current value is greater than the current value of the best-sales
    if sales > best_sales:
        best_sales = sales
    # checks if the value is less than the current value of worst_sales: if so, the worst_sales variable is updated
    elif sales < worst_sales:
        worst_sales = sales

profit_difference = best_sales - worst_sales

print("profit difference between best and worst sale:", profit_difference)
```

## Evidence of Code
<img width="1148" alt="Screen Shot 2023-08-22 at 20 36 12" src="https://github.com/maytemirabel/year-2/assets/105724334/ca54fe0a-561d-410f-82cf-d2c73a176d27">

#### Figure 2: Screenshot displaying code outcome
