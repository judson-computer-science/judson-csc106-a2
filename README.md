# Assignment 2 - Data Types and Operators
In this assignment you calculate the value of several items in a shopping cart and apply discounts to them where necessary.  The program should begin by taking the total number of items from the user as a command line parameter.
The number provided will determine how many times the program prompts the user for an item price.  For each item, the program will also prompt the user to determine if the item is on sale.  If it is, a discount of 10% will be applied to that item.  At the end of the program, a summary is printed including the total number of items, the total price, the number of discounted items and the total discount amount.

## Assignment Submission
You will submit your assignment using GitHub Classroom.  When you are finished and want to make your final submission, use the checkin comment "FINAL SUBMISSION":

        git add .
        git commit -m "FINAL SUBMISSION"
        git push origin main

Any submission not having this comment will be assumed to be a work-in-progress and therefore will be ignored.  This implies that you must make your final push with this commit comment before the deadline.

## Input
Your program will take 1 command line parameter representing the total number of items it should prompt to user for.  The program should validate that exactly 1 argument has been provided by the user before proceeding.

## Output
Your program will interact with the user as shown below:

    $> java ShoppingCart 3 4
    usage: java ShoppingCart <item count>
    
    $> java ShoppingCart    
    usage: java ShoppingCart <item count>

    $> java ShoppingCart 3
    
    Item 1 Price: 5.99
    On Sale? [true|false]: true
    
    Item 2 Price: 15.55
    On Sale? [true|false]: true
    
    Item 3 Price: 35.00
    On Sale? [true|false]: false
    
    Number of items: 3
    Number of sale items: 2
    Total price: $54.39
    Total discount: $ 2.15


## Implementation Notes
- It is ok for your program to assume that the input is an integer
- a discount of 10% should be applied to any item that is on sale
- your program should format the prices to 2 decimal places within a field that is at least 5 characters wide
- you must use the conditional operator in your program
- your class should be named 'ShoppingCart'
- rounding errors are acceptable
