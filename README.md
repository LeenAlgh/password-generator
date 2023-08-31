# password-generator
import random

# Defining the letters, digits and symbols that u want to have in the pass
uppercaseLetters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
lowercaseLetters = "abcdefghijklmnopqrstuvwxyz"
digit='0123456789'
symbols='%&/*#_-!'
# In case U don't want any type of it, set it to false
upper=True
lower=True
num=True
sym=True

all=''
#storing the TRUE variable in all 
if upper:
    all+=uppercaseLetters
if lower:
    all+=lowercaseLetters
if digit:
    all+=digit
if symbols:
    all+=symbols
#length of the password
length = 20
#generate 5 passwords
amount = 5

# Go through all using random function 
for x in range(amount):
    password = "".join(random.sample(all,length))
    print(password)
