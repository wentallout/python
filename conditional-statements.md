---
runme:
  id: 01HV1PBZPWQM94VSK9CYVQ52NJ
  version: v3
---

https://programming-24.mooc.fi/part-1/5-conditional-statements

```python {"id":"01HV1PJ9NFPCS1VB763KQQG2V0"}
number = input("Please type in a number:")

if number == "1984":
    print("Orwell")
```

## Get absolute number from input

```python {"id":"01HV1Q51TEY4RP4RR4B826Y36N"}
# Write your solution here
intNumber = int(input("Please type in a number:"))
absolute = 0

if(intNumber<0):
    absolute = intNumber * -1
else:
    absolute = intNumber

print(f"The absolute value of this number is {absolute}")
```

```python {"id":"01HV1RQ1MNCKJGCTV47QRKRYDP"}

number = int(input("Please type in a number: "))

if number < 10:
    print("This number is smaller than 1000")
    print("This number is smaller than 100")
    print("This number is smaller than 10")
elif number < 100:
    print("This number is smaller than 1000")
    print("This number is smaller than 100")
elif number < 1000:
    print("This number is smaller than 1000")
else:
    pass

print("Thank you!")


```

## Calculator

Please write a program which asks the user for two numbers and an operation. If the operation is add, multiply or subtract, the program should calculate and print out the result of the operation with the given numbers. If the user types in anything else, the program should print out nothing.

```python {"id":"01HV1S0NGYY3B3TYQS4EG2DKGZ"}
number1 = int(input("Number 1: "))
number2 = int(input("Number 2: "))
operation = input("Operation: ")

if operation == "add":
    result = number1 + number2
    print(f"{number1} + {number2} = {result}")
elif operation == "multiply":
    result = number1 * number2
    print(f"{number1} * {number2} = {result}")
elif operation == "subtract":
    result = number1 - number2
    print(f"{number1} - {number2} = {result}")
```

## Temperatures

Please write a program which asks the user for a temperature in degrees Fahrenheit, and then prints out the same in degrees Celsius. If the converted temperature falls below zero degrees Celsius, the program should also print out "Brr! It's cold in here!".

The formula for converting degrees Fahrenheit to degrees Celsius can be found easily by any search engine of your choice.

Two examples of expected behaviour:

```python {"id":"01HV1S3SX2B72NC4ER7Q4EMVYE"}
def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9


temperature_f = float(input("Please type in a temperature (F): "))
temperature_c = fahrenheit_to_celsius(temperature_f)

print(f"{temperature_f} degrees Fahrenheit equals {temperature_c} degrees Celsius")

if temperature_c < 0:
    print("Brr! It's cold in here!")

```

## Hourly wage

Please write a program which asks for the hourly wage, hours worked, and the day of the week. The program should then print out the daily wages, which equal hourly wage multiplied by hours worked, except on Sundays when the hourly wage is doubled.

```python {"id":"01HV1TYRV8Z3K56N98XHKR7B0X"}
# Write your solution here

hourlyWage = float(input("Hourly wage:"))
hoursWorked = int(input("Hours worked:"))
dayOfTheWeek = input("Day of the week:")

if dayOfTheWeek == "Sunday":
    hourlyWage = hourlyWage *2

dailyWages = hourlyWage * hoursWorked

print(f"Daily wages: {dailyWages} euros")
```

This program calculates the end of year bonus a customer receives on their loyalty card. The bonus is calculated with the following formula:

If there are less than a hundred points on the card, the bonus is 10 %
In any other case the bonus is 15 %

```python {"id":"01HV1V2NAEKJ1FDMVK0JMF7NQ8"}
# Fix the program
points = int(input("How many points are on your card? "))
if points < 100:
    points *= 1.1
    print("Your bonus is 10 %")
elif points >= 100:
    points *= 1.15
    print("Your bonus is 15 %")

print("You now have", points, "points")
```

```python {"id":"01HV1VS55NMWFK9THE7140TPGG"}

temp = int(input("Temperature?"))
isRain = input("Will it rain?")

print("Wear jeans and a T-shirt")

if temp <= 20:
    print("I recommend a jumper as well")

if temp <= 10:
    print("Take a jacket with you")

if temp <= 5:
    print("Make it a warm coat, actually")
    print("I think gloves are in order")


if isRain == "yes":
    print("Don't forget your umbrella!")

```