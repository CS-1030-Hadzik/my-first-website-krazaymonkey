---
layout: default
title: Projects
permalink: /projects/
---

[Back to Home Page](./index.markdown)
* * *

# My Programming Projects

> I've only learned the Python coding language so far.
> I will be learning JavaScript and C++ soon.
>

### Some Python Code I've Written

![Python Logo](/assets/images/python-logo-master-v3-TM-flattened.png)

 This is part of a game where you try to guess how much candy is in a jar

```py
def determine_winners(names, guesses, amount_of_candy):
    winners = []
    winners.append(names[0])
    #get the distance and use absolute value so we are just comparing distances
    winning_distance = abs(guesses[0] - amount_of_candy)
    for i in range(1, len(names)):
        dist = abs(guesses[i] - amount_of_candy)
        if dist == winning_distance:
            winners.append(names[i])
        elif dist < winning_distance:
            winners.clear()
            winning_distance = dist
            winners.append(names[i])

    return winners, winning_distance
```

This is from when I learned how to do if and while loops

```py
print("Welcome to the Kangaroo Zoo Cost Estimator! \nChoose an option: ")

calculate = 1

while calculate == 1:

    ticketCost = 0
    underThree = 6.00
    adults = 12.00
    frequentFlopperPass = 85.00
    underThreeFlopperPass = 50.00

    calculate = int(input("Estimate cost: 1 \nQuit: 2 or any other keystroke "))
    if calculate == 1:
        underThree *= int(input("How many guests are 3 and under? "))
        adults *= int(input("How many other guests will be jumping? "))

        response = input("Do you want to buy any Flopper Passes (yes or no)? ").lower()
        if response == "yes":
            frequentFlopperPass *= int(input("How many Adult passes(10 admissions)? "))
            underThreeFlopperPass *= int(input("How many under 3 passes(10 admissions)? "))
            ticketCost = underThree + adults + frequentFlopperPass + underThreeFlopperPass
        else:
            ticketCost = underThree + adults

        print("Your estimated cost: $", ticketCost)
    else:
        print("Thank you for using our calculator! ")
```
* * *