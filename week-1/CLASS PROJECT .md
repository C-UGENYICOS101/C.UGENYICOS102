```python
# Simple Interest Program
p = float(input("Enter Principal (P): "))
r = float(input("Enter Rate (R): "))
t = float(input("Enter Time (T): "))

# Calculation
a = p * (1 + (r / 100) * t)

print(f"The total amount (A) is: {a}")
```

    Enter Principal (P):  k
    


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    Cell In[1], line 2
          1 # Simple Interest Program
    ----> 2 p = float(input("Enter Principal (P): "))
          3 r = float(input("Enter Rate (R): "))
          4 t = float(input("Enter Time (T): "))
    

    ValueError: could not convert string to float: 'k'



```python
# Compound Interest Program
p = float(input("Enter Principal (P): "))
r = float(input("Enter annual interest Rate (R as decimal, e.g., 0.05 for 5%): "))
n = int(input("Enter number of times compounded per year (n): "))
t = float(input("Enter time in years (t): "))

# Calculation
a = p * (1 + r/n)**(n * t)

print(f"The compound interest amount (A) is: {a}")
```


```python
# Annuity Plan Program
pmt = float(input("Enter periodic payment (PMT): "))
r = float(input("Enter annual interest Rate (R as decimal): "))
n = int(input("Enter number of payments per year (n): "))
t = float(input("Enter time in years (t): "))

# Calculation
# Breaking it down for readability (Best Practice)
rate_per_period = r / n
number_of_periods = n * t

a = pmt * (((1 + rate_per_period)**number_of_periods - 1) / rate_per_period)

print(f"The total annuity amount (A) is: {a}")
```
