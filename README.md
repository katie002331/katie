import random
import string

def generate_random_string(length):
    characters = string.ascii_lowercase
    random_string = ''.join(random.choice(characters) for i in range(length))
    return random_string

def is_palindrome(input_string):
    reversed_string = input_string[::-1]
    return input_string == reversed_string

string_length = 10

random_string = generate_random_string(string_length)
print("随机生成的字符串：", random_string)

if is_palindrome(random_string):
    print("这个字符串是回文。")
else:
    print("这个字符串不是回文。")
