---
runme:
  id: 01HV1WXWNDG999YFKA92J574MV
  version: v3
---

Please write a program which estimates a user's typical food expenditure.

The program asks the user how many times a week they eat at the student cafeteria. Then it asks for the price of a typical student lunch, and for money spent on groceries during the week.

Based on this information the program calculates the user's typical food expenditure both weekly and daily.

```python {"id":"01HV1WYQVAFN3S74XHTB4SA25C"}
# Write your solution here
cafeteriaVisitPerWeek = int(input("How many times a week do you eat at the student cafeteria? "))

lunchPrice = float(input("The price of a typical student lunch?"))
moneyPerWeek = float(input("How much money do you spend of groceries in a week?"))

weeklyExpenditure = (cafeteriaVisitPerWeek * lunchPrice) + moneyPerWeek
dailyExpenditure = weeklyExpenditure / 7

print(f"Daily: {dailyExpenditure} euros")
print(f"Weekly: {weeklyExpenditure} euros")
```

Please write a program which asks for the number of students on a course and the desired group size. The program will then print out the number of groups formed from the students on the course. If the division is not even, one of the groups may have fewer members than specified.

```python {"id":"01HV1WZ7528Y00VV2NRYPST5FS"}
students_count = int(input("How many students on the course? "))
group_size = int(input("Desired group size? "))

groups_formed_count = students_count // group_size
remaining_students = students_count % group_size

if remaining_students > 0:
    groups_formed_count += 1

print(f"Number of groups formed: {groups_formed_count}")
```