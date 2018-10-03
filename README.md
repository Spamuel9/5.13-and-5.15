# 5.13-and-5.15
import random

num_two = 0
num_three = 0
num_four = 0
num_five = 0
num_sixes = 0
num_sevens = 0
num_eight = 0
num_nine = 0
num_ten = 0
num_eleven = 0
num_twelve = 0
num_rolls = int(input('Enter number of rolls:\n'))
while num_rolls >= 1:
    for i in range(num_rolls):
        die1 = random.randint(1,6)
        die2 = random.randint(1,6)
        roll_total = die1 + die2
        if roll_total == 2:
            num_two = num_two + 1
        if roll_total == 3:
            num_three = num_three + 1
        if roll_total == 4:
            num_four = num_four + 1    
        if roll_total == 5:
            num_five = num_five + 1
        if roll_total == 6:
            num_sixes = num_sixes + 1
        if roll_total == 7:
            num_sevens = num_sevens + 1
        if roll_total == 8:
            num_eight = num_eight + 1
        if roll_total == 9:
            num_nine = num_nine + 1
        if roll_total == 10:
            num_ten = num_ten + 1
        if roll_total == 11:
            num_eleven = num_eleven + 1
        if roll_total == 12:
            num_twelve = num_twelve + 1
        print('Roll %d is %d (%d + %d)' % (i, roll_total, die1, die2))
        num_rolls = num_rolls - 1
    print('\nDice roll histogram::')
    print('2s:', num_two)
    print('3s:', num_three * '*')
    print('4s:', num_four * '*')
    print('5s:', num_five * '*')
    print('6s:', num_sixes * '*')
    print('7s:', num_sevens * '*')
    print('8s:', num_eight * '*')
    print('9s:', num_nine * '*')
    print('10s:', num_ten * '*')
    print('11s:', num_eleven * '*')
    print('12s:', num_twelve * '*')
