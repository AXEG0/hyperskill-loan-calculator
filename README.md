Example 1: calculating differentiated payments

Python Run command in Terminal:
```
> python creditcalc.py --type=diff --principal=1000000 --periods=10 --interest=10
Month 1: payment is 108334
Month 2: payment is 107500
Month 3: payment is 106667
Month 4: payment is 105834
Month 5: payment is 105000
Month 6: payment is 104167
Month 7: payment is 103334
Month 8: payment is 102500
Month 9: payment is 101667
Month 10: payment is 100834

Overpayment = 45837
```
In this example, the user wants to take a loan with differentiated payments. User know the principal, the count of periods, and interest, which are 1,000,000, 10 months, and 10%, respectively.

---------------------------------
Example 2: calculate the annuity payment for a 60-month (5-year) loan with a principal amount of 1,000,000 at 10% interest

Python Run command in Terminal:
```
> python creditcalc.py --type=annuity --principal=1000000 --periods=60 --interest=10
Your annuity payment = 21248!
Overpayment = 274880
```
---------------------------------
Example 3: fewer than four arguments are given

Python Run command in Terminal:
```
> python creditcalc.py --type=diff --principal=1000000 --payment=104000
Incorrect parameters.
```
---------------------------------
Example 4: calculate differentiated payments given a principal of 500,000 over 8 months at an interest rate of 7.8%

Python Run command in Terminal:
```
> python creditcalc.py --type=diff --principal=500000 --periods=8 --interest=7.8
Month 1: payment is 65750
Month 2: payment is 65344
Month 3: payment is 64938
Month 4: payment is 64532
Month 5: payment is 64125
Month 6: payment is 63719
Month 7: payment is 63313
Month 8: payment is 62907

Overpayment = 14628
```
---------------------------------
Example 5: calculate the principal for a user paying 8,722 per month for 120 months (10 years) at 5.6% interest

Python Run command in Terminal:
```
> python creditcalc.py --type=annuity --payment=8722 --periods=120 --interest=5.6
Your loan principal = 800018!
Overpayment = 246622
```
---------------------------------
Example 6: calculate how long it will take to repay a loan with 500,000 principal, monthly payment of 23,000, and 7.8% interest

Python Run command in Terminal:
```
> python creditcalc.py --type=annuity --principal=500000 --payment=23000 --interest=7.8
It will take 2 years to repay this loan!
Overpayment = 52000
```
