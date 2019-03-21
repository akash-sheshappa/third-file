"""
Objective: Number pattern generation

Description : Creates a triangle pattern of numbers

@author: Akash Sheshappa

Version : 3.7

Date: 13/04/2019

Testcases:
Positive number  => All Scenarios - Tested OK
Negative => Tested Not OK - Error
Zero => Test OK
Triangle pattern of special character => All Scenarios - Tested OK
Triangle pattern of number => All Scenarios - Tested OK
Traiangle pattern of Alphabets => All Scenarios - Tested OK
Circular pattern of characters press => All Scenarios - Tested OK

Initial Static Code Analysis Score - > -3.5/10
Final Static Code Analysis Score - >2.64/10   """

import math

#Function to demonstrate printing pattern triangle
def num_pat(n):
    """initialising starting number"""
    num = 1
    # outer loop to handle number of rows
    for i in range(0, n):
        # re assigning num
        num = 1
        # inner loop to handle number of columns
        for j in range(0, i+1):
            # printing number
            print(num, end=" ")
            # incrementing number at each column
            num = num + 1
            # ending line after each row
        print("\r")


#Function to print a triangle of special charachter
def triangle(n, c):
    """initialising starting number"""
    # number of spaces
    k = 2*n - 2
    # outer loop to handle number of rows
    for i in range(0, n):
        # inner loop to handle number spaces
        for j in range(0, k):
            print(end="")
            # decrementing k after each loop
            k = k - 1
            # inner loop to handle number of columns
        for j in range(0, i+1):
                # printing stars
                print(c, end=" ")
                # ending line after each row
                
        print("\r")

def alphapat(n):
    """initialising starting number"""
    # initializing value corresponding to 'A'
    # ASCII value
    num = 65
    # outer loop to handle number of rows
    # 5 in this case
    for i in range(0, n):
        # inner loop to handle number of columns
        # values changing acc. to outer loop
        for j in range(0, i+1):
            # explicitely converting to char
            ch = chr(num)
            # printing char value
            print(ch, end=" ")
        # incrementing number
        num = num + 1
        
        # ending line after each row
        print("\r")

# function to print circle pattern
def printPattern(radius, smb):
    """initialising starting number"""
    # dist represents distance to the center
    # for horizontal movement
    for i in range((2 * radius)+1): 
        # for vertical movement
        for j in range((2 * radius)+1):
            
            dist = math.sqrt((i - radius) * (i - radius) + (j - radius) * (j - radius))
            # dist should be in the
            # range (radius - 0.5)
            # and (radius + 0.5) to print stars(*)
            if (dist > radius - 0.5 and dist < radius + 0.5):
                print(smb, end="")
            else:
                print(" ", end="")


        print()


while True:   #to make the loop forever
 X = input("If you want to print a triangle pattern of special character press --> 1 \nif you want to print a triangle pattern of number press --> 2\nIf you want a traiangle pattern of Alphabets press --> 3 \nIf you want a Circular pattern of characters press --> 4 \n ")
 N = int(X)

 if N == 1:
    Col = int(input("How many columns do you need "))
    spl = input("Enter the Character you wish to print ")
    triangle(Col, spl)

 elif N == 2:
    Cl = int(input("How many rows of Number patterns do you want "))
    num_pat(Cl)
 elif N == 3:
    #alphapat(input("How many columns do you need "))
    Alp = int(input("How many columns do you need "))
    if Alp > 26:
        print("There are only 24 charchters in the English alphabet, number of rows can't be more than 24")
    else:
        alphapat(Alp)
 elif N == 4:
    radius = int(input("Enter the Radius of the circle pattern "))
    smbl = input("Enter the characters you would like to print")
    printPattern(radius, smbl)
