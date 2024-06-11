# Captcha.py
#Develop a simple Captcha generator. #You have to generate a captcha  of 5 #characters including(A-Z,a-z,0-9).
import random
import string

def generate_captcha(length=6):
    # Define the character set (uppercase letters and digits)
    char_set = string.ascii_uppercase + string.digits
    
    # Generate a random captcha string
    captcha = ''.join(random.choice(char_set) for _ in range(length))
    
    return captcha

# Test the function by generating and printing 5 captchas
for _ in range(5):
    print(generate_captcha())
