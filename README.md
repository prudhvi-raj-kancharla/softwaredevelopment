# softwaredevelopment
# This code generates a random password
import random
import string

def generate_password(length):
    """Generates a random password of a specified length."""

    characters = string.ascii_letters + string.digits + string.punctuation
    password = "".join(random.choice(characters) for i in range(length))
    return password

# Generate a password of length 12
password = generate_password(12)
print(password)
