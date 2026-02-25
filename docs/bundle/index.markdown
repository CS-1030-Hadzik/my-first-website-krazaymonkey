---
layout: default
title: "Home Page"
---

This website is a work in progress and will be updated periodically

[Link to the Jekyll info](./about.markdown)

# About Me

  Hi! My name is Tiffany and I'm a student at Weber State University, studying 
  Computer Science. I've created this website as an assignment for a class and 
  also to showcase some of my skills. Thank you to Scott Hadzik for creating the
  base code and assignment.

## My First Website

  The below link is a website I created through Weebly.com while in High School to showcase different things about my time in school.

[Link to my High School Portfolio](https://twhsportfolio.weebly.com/).


### Quotes I Like

*   Even the darkest night will end and the sun will rise. - Herbert Kretzmer
*   The only appropriate state of the heart is joy... The perfect moment is now. Be glad of it. - Terry Pratchett
*   When something is important enough, you do it even if the odds are not in your favor.
*   Embrace all living creatures and the whole of nature in its beauty. - Albert Einstein

* * *

# Programming

> I've only learned the Python coding language so far.
> I will be learning JavaScript and C++ soon.

### Some Python Code I've Written

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

### Table of Games

| Game Name         | Series?   | Have I completed?          |
|:------------------|:----------|:---------------------------|
| Mass Effect       | Yes       | All `4` games              |
| Horizon: Zero Dawn| Yes       | Yes, waiting for 3         |
| Stardew Valley    | `No`      | Yes, still playing for fun |
| Fallout 4         | Yes       | `No`, playing now          |

### There's a horizontal rule below this.

* * *
##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```
