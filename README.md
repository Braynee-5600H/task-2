# task-2

import random
import string

def Generate_Password(len):
    characters = string.ascii_letters + string.digits + string.punctuation
    Password = ''.join(random.choice(characters) for _ in range(len))
    return Password


Password_length = int(input("Enter the required length of the password: "))


Password = Generate_Password(Password_length)
print("Generated Password is: ",Password)
