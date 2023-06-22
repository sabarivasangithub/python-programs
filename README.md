# python-programs
# square root 
import math
num = int(input("enter the number: "))
print("The square root of the number is: ", math.sqrt(int(num)))
# area of triangle
import math
breadth = int(input("enter the breadth: "))
height = int(input("enter the height: "))
print("The area of the triangle is: ", 1/2*breadth*height)
# solving quadratic equation using cmath
import cmath
a = int(input("enter the 1st number: "))
b = int(input("enter the 2nd number: "))
c = int(input("enter the 3rd number: "))  # formula is -b +- (b**2 - 4ac)**1/2/2a
d = b**2 - 4*a*c
sol1 = (-b + cmath.sqrt(d))/2*a
sol2 = (-b - cmath.sqrt(d))/2*a
print('The solution are {0} and {1}'.format(sol1,sol2))
# python program to swap two variables
var1 = input("enter the 1st variable: ")
var2 = input("enter the 2nd variable: ")
temp = var1
var1 = var2
var2 = temp
print("the two variables after swapping are {0} and {1}" .format(var1,var2))
# generate random number
import random
print(random.randint(0,10))
# convert kilometer to mile
km = float(input("enter the kilometer: "))
conversion_factor = 1.60934
print("%0.2f kilometer is equals to %0.2f miles" %(km,km/conversion_factor))
# convert celcius to farenheit
celcius = float(input("enter the degree celcius: "))
##1 celcius = 33.8 fahrenheit
##fahrenheit = celsius * 1.8 + 32 
fahrenheit = celcius * 1.8 +32
print(fahrenheit)
# Python Program to Check if a Number is Positive, Negative or 0
num = int(input("enter the number: "))
if num > 0 :
    print("{} is positive".format(num))
elif num < 0 :
    print("{} is negative".format(num))
else:
    print("{} is neither positve nor negative" .format(num))
# Python Program to Check if a Number is Odd or Even
num = int(input("enter the number: "))
if num%2 == 0 :
    print("the given number is even")
elif num%2 != 0 :
    print("the given number is odd")
else :
    print("try other number")
# Python Program to Check Leap Year
year = int(input("enter the year: "))
if year%100 == 0 and year%400 == 0 :
    print("{} is a leap year".format(year))
elif year%100 != 0 and year%4 == 0 :
    print("{} is a leap year".format(year))
else :
    print("{} is not a leap year".format(year))
# largest among 3 numbers
a = float(input("enter the 1st number a: "))
b = float(input("enter the 2nd number b: "))
c = float(input("enter the 3rd number c: "))
if a > b and a > c :
    print("a is greatest")
elif b > c:
    print("b is greatest")
else:
    print("c is greatest")
********************************************************************************************************
# check prime number or not
num = int(input("enter the number: "))
if num == 1 :
    print("not prime number")
elif num>1 :
    for i in range(2,num):
        if num%i == 0 :
            print("not prime number")
            break
        else:
            print("it is a prime number")
            break
else:
    print("not a prime number")
# Python Program to find the L.C.M. of two input number

def compute_lcm(x, y):

   '''choose the greater number'''
   if x > y:
       greater = x
   else:
       greater = y

   while(True):
       if((greater % x == 0) and (greater % y == 0)):
           lcm = greater
           break
       greater += 1

   return lcm

num1 = 54
num2 = 24

print("The L.C.M. is", compute_lcm(num1, num2))
# prime numbers in a given range
start = int(input("enter the starting number: "))
end = int(input("enter the ending number: "))
flag = True
for i in range(start,end+1):
    for j in range(2,i):
        if i%j == 0 :
            print("{} not a prime number".format(i))
            break
    else:
        print("{} is a prime number".format(i))
# armstrong numbers between two intervals \\\ The Armstrong number in Python is the number in which the sum of each digit powered to the total number of digits is the same as the given number \\\
num = int(input("enter the number: "))
sum = 0
for i in str(num):
    sum += int(i)**len(str(num))
if sum == num:
    print("{} is a armstrong number".format(num))
else:
    print("{} is not a armstrong number".format(num))
# program to express a number as a sum of two prime numbers
num = int(input('Enter the Number : '))

arr = []
for i in range(2,num+1):
    flag = 0
    for j in range(2,i):
        if i%j == 0 :
            flag = 1
    if flag == 0 :
        arr.append(i)
print(arr)
flag = 0
for a in range(len(arr)):
    for b in range(a+1,len(arr)):
        if arr[a]+arr[b]==num:
            print("{} and {} combines and give the value of {}".format(arr[a],arr[b],num))
            flag = 1
if flag == 0:
    print("sorry! there is no such combinations")


























