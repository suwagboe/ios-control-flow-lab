# Control Flow Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")
```

- A
- B
- C
- D
```
A , C, D 
```
***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}
```

- appInfo.0 hasn't released yet
- myCoolApp hasn't released yet
- Thanks for looking at myCoolApp!
- I'm not quite sure what you are looking at
- It will give a compile-time error

```
myCoolApp hasn't released yet
Thanks for looking at myCoolApp!

```
***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
```
D
```
```
***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}
```

- No parentheses around the conditions
- No opening and closing brackets in each of the cases
- No default case in the switch statement
- No print statement right outside the switch statement
```
- No default case in the switch statement

```
***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

// enter code below
```
```
let currentWeather = "rain"

switch currentWeather {
case "rain":
 print("don't forget your umbrella")
case "sunny":
 print("don't forget your sunscreen for this sunny day")
case "snow":
 print("it's snowing so it's time for hot chocolate")

Default: 
Print("either way you're alive so enjoy the weather today")
}
```
***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

// enter code below
```
```
var fullName = "\(firstName) \(lastName)"
print(fullName)
```

***

## Question 7

Convert the if/else statement below into a switch statement.

```swift
if temperatureInFahrenheit <= 40 {
 print("It's cold out.")
} else if temperatureInFahrenheit >= 85 {
 print("It's really warm.")
} else {
 print("Weather is moderate.")
}

//Re-written statement here

```
```
Switch temperatureInFahrenheit{
Case  40:
Print ("it's cold out")
Case 80:
Print("it's really warm")
Default:
("Weather is moderate")
}

```

***

## Question 8

Complete the following code so that "You win!" is printed.

```swift
if {
 print("You win!")
} 
else {
 print("You lose!")
}
```
```
let testScore = 90
if testScore == 90 {
 print("You win!")
}
else {
 print("You lose!")
}

```
***

## Question 9

Given a variable called numberOfSides, write code using a switch so that it prints out the name of the shape. Account for shapes with 3 to 10 sides and print an error message if out of range.

var numberOfSides = 6

```swift
Example 1:

Input:
var numberOfSides = 4

Output:
Square

Example 2:

Input:
var numberOfSides = 2

Output:
Error

```
```
var numberOfSides = 4

switch numberOfSides {
case 3:
    print("triangle")
    case 4:
    print("Square")
    case 5:
    print("pentagon")
    case 6:
    print("hexagon")
    case 7:
    print("heptagon")
    case 8:
    print("octagon")
    case 9:
    print("nonagon")
    case 10:
    print("decagon")
default:
    print("Error")
}

```

***

## Question 10

Create a switch statement that will convert a number grade into a letter grade as shown below:

```swift
Numeric Score 	Letter Grade
100 	A+
90 - 99	A
80 - 89	B
70 - 79 	C
65 - 69 	D
Below 65 	F
```
```
var yourScore = 95
switch yourScore  {
case 100:
    print("A+")
case 90..<99:
    print("B")
case 88..<89:
    print("B")
case 70..<79 :
    print("C")
case 65..<69 :
    print("D")
case ..<65 :
    print("F")
default:
    print("Error")
}

```
***

## Question 11 (!!!)

What is wrong with the block of code below?  Correct it so it behaves as expected.

```swift
let firstName = "Peter"

if firstName == "Peter" {
 let lastName = "Gabriel"
} else if firstName == "Phil" {
 let lastName = "Collins"
}
let fullName = (firstName + " " + lastName)
```
```
let firstName = "Peter"
 var lastName = ""

if firstName == "Peter" {
  lastName = "Gabriel"
} else if firstName == "Phil" {
  lastName = "Collins"
}
let fullName = firstName + " " + lastName
```
***

## Question 12 (work on if else statments)

Write an if statement that prints out what decade of life someone is in (e.g "You are in your twenties). Then, write it as a switch statement.

```swift
let nameAndBirthYear: (String, Int)

```
```
var birthYear = 1997

if birthYear 1990..<2000{
print ("You are in your twenties")
}
if birthYear 2001-2019 {
print("You are in your teens")
}

switch birthYear
case 1990..<2000 :
    print("You are in your twenties")
    case 2000..<2019 :
    print("You are in your teens")
default:
    print("Error")
}



```
***


## Question 13

Consider the below switch statement. What should your system currently print?

```swift
let number = 42

switch number {
case 365:
 print("Days in year")
case 1024:
 print("Bytes in a Kilobyte")
case 0:
 print("Where arrays start")
case 42:
 print("The answer to life, the universe and everything")
default:
 print("Some uninteresting number")
```
What happens when you change number to:

-a. 365?

-b. 1024?

-c. 65?

What happens when you remove the default clause?

```
The first thing this would print is :The answer to life, the universe and everything

second thing is: Days in year

third thing is: Bytes in a Kilobyte

fourth thing is :
Some uninteresting number

when the default clause is removed the file complies and it is not exhausted 
```

***


## Question 14

Consider the variable below called population and the if-condition.

a. Add an else-if-condition that states if population is less than 10000 but greater than 5000, then message changes to say it's "a medium size town".

b. Add an else-condition where message changes to say it's a mid-size town.

c. Convert your final if-else statement to a switch statement.

```swift
var population: Int = 10000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
} else if 
```
```
var population = 6000

if population > 10000 {
 print("\(population) is a large town")
} else if 5_000 ..< 10_000 {
 print("a medium size town")
 } else {
 print("Its a mid-size town")
}
```
***

## Question 15

Complete the code below so that it prints out and tells the user if the sum of the two numbers in the tuple is at least 15.

a. Using a conditional

b. Using a switch statement

```swifts
let myTuple: (Int, Int) = (5, 10)
```
```
A.
if my myTuple <= 15 {
print("The sum of the two number in the tuple is at least 15")
} else {
print("Try again")
}

B.
let myTuple = 10 + 5
switch myTuple
{
case myTuple <= 15 
 print("The sum of the numbers is at least 15")
 default:
 print("Try again")
}

```
***
