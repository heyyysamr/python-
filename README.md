print("Hello World!")
def calculator():
    num1 = float(input("Pehla number daalo: "))
    op = input("Operator (+, -, *, /): ")
    num2 = float(input("Dusra number daalo: "))
    
    if op == '+':
        print(f"Result: {num1 + num2}")
    elif op == '-':
        print(f"Result: {num1 - num2}")
    elif op == '*':
        print(f"Result: {num1 * num2}")
    elif op == '/':
        if num2 != 0:
            print(f"Result: {num1 / num2}")
        else:
            print("Zero se divide nahi kar sakte!")
    else:
        print("Galat operator!")

calculator()
import random

number = random.randint(1, 100)
attempts = 0

print("1-100 ke beech number guess karo!")

while True:
    guess = int(input("Apna guess daalo: "))
    attempts += 1
    
    if guess < number:
        print("Thoda upar jao!")
    elif guess > number:
        print("Thoda neeche aao!")
    else:
        print(f"Badhiya! {attempts} attempts mein sahi guess!")
        break
        # List banaye
fruits = ["apple", "banana", "cherry"]

# Add karo
fruits.append("orange")
print("List:", fruits)

# Loop karo
for fruit in fruits:
    print(f"I like {fruit}")

# Length check
print(f"Total fruits: {len(fruits)}")
