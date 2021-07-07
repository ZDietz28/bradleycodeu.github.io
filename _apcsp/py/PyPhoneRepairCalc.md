---
layout: project
category: py
title: Phone Repair Calc
---
Read these tutorials:
- [Python Functions](/apcsp\py\pythonfunctions)
- [Python Conditionals](https://www.w3schools.com/python/python_conditions.asp)

Create a Phone Repair Calculator that predicts the amount of profit you can earn by buying and repairing phones with cracked screens.

Fill in ALL 10 blanks in the starter code with the correct code.
Blanks look like this: ???

When finished, type in both Test Runs to make sure your code works correctly. If no errors, submit to replit classroom and then go to the Canvas assignment and say "done"

Test Run 1:
```
How much $ can you invest in cracked-screen phones:
999.99
Cracked-screen phone price:
100.01
Repair kit price:
25.25
Sale price for fixed phone:
149.99
-----Re$ult-----
You earned $173.11 in profit
```

Test Run 2:
```
How much $ can you invest:
-99
Cracked-screen phone price:
-33
Repair kit price:
-11
Sale price for fixed phone:
987654321
-----Re$ult-----
You earned $0.0 in profit
```

STARTER CODE:
```python
# Fill in ALL 10 blanks with the correct code.
# Blanks look like this: ???

# the sellPhones function tells you how much money you can earn
# requires two arguments: myPhones, salePrice
def sellPhones(myPhones, salePrice):
  #convert myPhones to an int
  myPhones = int(myPhones)
  #convert salePrice to a float
  ???
  #myPhones multiplied by salePrice equals myMoney
  ???
  #if myMoney is less than 0
  if ???:
      #then myMoney equals 0
      myMoney = 0
  return myMoney


# the buyPhones function tells you how many phones you can afford to buy
# requires two arguments: myDollars, phonePrice
def buyPhones(myDollars, phonePrice):
  #convert myDollars to a float
  myDollars = float(myDollars)
  #convert phonePrice to a float
  ???
  #create new variable amountOfPhones, set it to 0
  amountOfPhones = 0
  #if phonePrice is greater than 0
  if ???:
      #then myDollars divided by phonePrice equals amountOfPhones
      amountOfPhones = myDollars / phonePrice
  #if amountOfPhones is less than 0
  if ???:
      #then amountOfPhones equals 0
      amountOfPhones = 0
  #convert amountOfPhones to an int
  ???
  return amountOfPhones


# this function calculates and returns the profit
# requires 4 arguments: investMoney, usedPrice, repairPrice, salePrice
def calculateProfit(investMoney, usedPrice, repairPrice, salePrice):
  #create a new variable named cost.
  #usedPrice plus repairPrice equals cost
  ???
  #find out how many phones you can buy
  numberPhones = buyPhones(investMoney, cost)
  #create a new variable named moneySpent.
  #usedPrice*numberPhones plus repairPrice*numberPhones equals moneySpent
  ???
  #find out how much money you earned
  moneyEarned = sellPhones(numberPhones, salePrice)
  #create a new variable named profit.
  #profit is moneyEarned minus moneySpent
  ???
  return profit


# ------------------------------------
# YOU ARE DONE!
# do NOT edit the following code!
def main():
  print("How much $ can you invest: ")
  investMoney = float(input())
  print("Cracked-screen phone price: ")
  usedPrice = float(input())
  print("Repair kit price: ")
  repairPrice = float(input())
  print("Sale price for fixed phone: ")
  salePrice = float(input())
  profit = calculateProfit(investMoney, usedPrice, repairPrice, salePrice)
  print("-----Re$ult-----\nYou earned $"+str(round(profit,2))+" in profit")
main()

```
