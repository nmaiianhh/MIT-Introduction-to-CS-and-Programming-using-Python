# -*- coding: utf-8 -*-
"""
Created on Fri Jan  9 17:14:39 2026

@author: nmaia
"""
# first
# num1 = input("Type a number: ")
# print(5*num1)
# # second
# num2 = int(input("Type another number: "))
# print(5*num2)

############################################################################################################

# # third
# s = "I can _ better than you!"
# text = input("type a verb: ")
# print(5*(text+" "))
# s = s[0:6] + text + s[7:len(s)]
# print(s)

# # third - to remove the extra " " at the end
# text = input("type a verb: ")
# a = 5*(text+" ")
# print(a[0:len(a)-1])

# # another way to do third question
# question = input('Choose a verb: ')
# print('I can', question, 'better than you!')

############################################################################################################

# # Newton's method to find cube root
# x = float(input('What x to find the root of? '))
# g = float(input('What guess to start with? '))

# print('Current estimate cube = ', g**3)
# next_g = g - ((g**3 - x)/(3*g**2))
# print('Next guess to try = ', next_g)

############################################################################################################

# F-STRINGS
# num = 3000
# fraction = 1/3
# print(num*fraction, 'is', fraction*100, '% of', num)
# print(num*fraction, 'is', str(fraction*100) + '% of', num)
# print(f'{num*fraction} is {fraction*100}% of {num}')

############################################################################################################

# # Boolean
# pset_time = 15
# sleep_time = 8
# print(sleep_time>pset_time)
# derive = True
# drink = False
# both = drink and derive
# print(both)


# Example
# secret = 28
# text = input('Guess the secret number: ')
# print(secret == text)


# scret = 5
# guess = int(input("Please guess another number: "))
# print (guess == scret)

############################################################################################################

# # BRANCHING
# # pset_time = 20
# sleep_time = 2
# if (pset_time + sleep_time) > 24:
#     print('Impossible!')
# elif (pset_time + sleep_time) >= 24:
#     print('Full schedule!')
# else:
#     leftover = abs(24 - pset_time - sleep_time)
#     print(leftover, 'hours of free time')
# print('end of day')
# # note: for the above, ">=" means "=", as "=" is syntax error

############################################################################################################

# # Nested branching
# x = float(input('Type a number for x: '))
# y = float(input('Tyoe a number for y: '))
# if x==y:
#     print('x and y are equal.')
#     if y != 0:
#         print('therefore x/y is', x/y)
# elif x < y:
#     print('x is smaller.')
# else:
#     print('y is smaller')
# print('thanks!')
# # note: 'y != 0!' means 'y is not qual to 0'

############################################################################################################

# # example 1
# secret = 113
# guess = float(input('Guess the secret number: '))
# if secret == guess:
#     print('Correct!')
# elif secret > guess:
#     print('Too low!')
# else:
#     print('Too high!')

############################################################################################################

# # Part A: Saving for a House
# yearly_salary = float(input('Enter your yearly salary: '))
# portion_saved = float(input('Enter the percent of your salary to save, as a decimal: '))

# amount_saved_per_year = yearly_salary * portion_saved
# amount_saved_per_month = amount_saved_per_year/12

# cost_of_dream_home = float(input('Enter the cost of your dream home: '))
# portion_down_payment = 0.25
# cost_of_down_payment = portion_down_payment*cost_of_dream_home

# print("cost of down payment", cost_of_down_payment)

# annual_return_on_investment = 0.05
# monthly_return_on_investment = annual_return_on_investment/12

# current_amount_saved = 0

# month = 0

# while current_amount_saved < cost_of_down_payment:
#     print("month", month)
#     print("current amount saved", current_amount_saved)
#     interest_earned = current_amount_saved*monthly_return_on_investment
#     current_amount_saved = current_amount_saved + amount_saved_per_month + interest_earned
#     month = month + 1
    
# print(month)

# year = month/12
# print(year)

############################################################################################################

# # Part B: Saving with a raise
# yearly_salary = float(input('Enter your yearly salary: '))
# portion_saved = float(input('Enter the percent of your salary to save, as a decimal: '))

# cost_of_dream_home = float(input('Enter the cost of your dream home: '))
# portion_down_payment = 0.25
# cost_of_down_payment = portion_down_payment*cost_of_dream_home

# annual_rate_of_return = 0.05
# monthly_rate_of_return = annual_rate_of_return/12

# semi_annual_raise = float(input('Enter the semi-annual raise, as a decimal: '))
    
# current_amount_saved = 0 
# month = 0

# while current_amount_saved < cost_of_down_payment:
#     month += 1
#     monthly_salary = yearly_salary / 12
    
#     interest_earned = current_amount_saved*monthly_rate_of_return
#     earning_saved = monthly_salary*portion_saved
#     current_amount_saved += interest_earned + earning_saved
    
#     if month % 6 == 0:
#         yearly_salary *= 1+semi_annual_raise

# print('Number of months: ', month)

#######################################

# CHATGPT PART B
# yearly_salary = float(input("Enter your starting salary: "))
# portion_saved = float(input("Enter the percent of your salary to save, as a decimal: "))
# cost_of_dream_home = float(input("Enter the cost of your dream home: "))
# semi_annual_raise = float(input("Enter the semi-annual raise, as a decimal: "))

# # Constants
# portion_down_payment = 0.25
# annual_return = 0.05
# monthly_return = annual_return / 12

# # Calculations
# down_payment = cost_of_dream_home * portion_down_payment
# current_savings = 0
# months = 0

# while current_savings < down_payment:
#     months += 1

#     # Monthly savings
#     monthly_salary = yearly_salary / 12
#     current_savings += current_savings * monthly_return
#     current_savings += monthly_salary * portion_saved

#     # Apply raise every 6 months
#     if months % 6 == 0:
#         yearly_salary += yearly_salary * semi_annual_raise

# print("Number of months:", months)

############################################################################################################

#Part C: Choosing an Interest Rate - CHATGPT
# User input
initial_deposit = float(input("Enter the initial deposit: "))

# Constants
cost_of_house = 800000
portion_down_payment = 0.25
down_payment = cost_of_house * portion_down_payment
months = 36
epsilon = 100

# If already enough with no interest
if initial_deposit >= down_payment - epsilon:
    r = 0.0
    steps = 0
else:
    low = 0.0
    high = 1.0
    steps = 0
    r = None

    while low <= high:
        steps += 1
        guess = (low + high) / 2
        current_savings = initial_deposit

        # simulate 36 months of compound interest
        for _ in range(months):
            current_savings += current_savings * (guess / 12)

        if abs(current_savings - down_payment) <= epsilon:
            r = guess
            break
        elif current_savings < down_payment:
            low = guess
        else:
            high = guess

        if steps > 1000:
            break

# Check if impossible
if r is None:
    print("Best savings rate: ", r)
    print("Steps in bisection search: ", steps)
else:
    print("Best savings rate: ", round(r, 4))
    print("Steps in bisection search: ", steps)
