'''import random
secret_number = random.randint(1, 100)
print("===================================")
print("      NUMBER GUESSING GAME")
print("===================================")
print("I have selected a number between 1 and 100.")
print("Try to guess it!")
attempts = 0
while True:
    try:
        guess = int(input("\nEnter your guess: "))
        attempts += 1

        if guess < secret_number:
            print(" Too low! Try again.")

        elif guess > secret_number:
            print(" Too high! Try again.")

        else:
            print("\n Congratulations!")
            print(f"You guessed the correct number: {secret_number}")
            print(f"Total attempts: {attempts}")
            break

    except ValueError:
        print(" Please enter a valid integer.")'''
        

'''correct_pin = "1234"
balance = 5000

print("=================================")
print("      WELCOME TO ATM")
print("=================================")

pin = input("Enter your 4-digit PIN: ")

if pin == correct_pin:
    print("\nLogin Successful!")

    while True:
        print("\n========== ATM MENU ==========")
        print("1. Check Balance")
        print("2. Deposit Money")
        print("3. Withdraw Money")
        print("4. Exit")

        choice = input("Enter your choice (1-4): ")

        if choice == "1":
            print(f"\nYour current balance is: ₹{balance}")

        elif choice == "2":
            amount = float(input("Enter amount to deposit: ₹"))

            if amount > 0:
                balance += amount
                print(f"₹{amount} deposited successfully.")
                print(f"Updated Balance: ₹{balance}")
            else:
                print("Invalid amount!")

        elif choice == "3":
            amount = float(input("Enter amount to withdraw: ₹"))

            if amount <= 0:
                print("Invalid amount!")

            elif amount > balance:
                print("Insufficient balance!")

            else:
                balance -= amount
                print(f"₹{amount} withdrawn successfully.")
                print(f"Remaining Balance: ₹{balance}")

        elif choice == "4":
            print("\nThank you for using our ATM!")
            print("Have a nice day!")
            break

        else:
            print("Invalid choice! Please select between 1 and 4.")

else:
    print("\nIncorrect PIN! Access Denied.")'''
    

'''print("=================================")
print("      BASIC CALCULATOR")
print("=================================")

num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

operator = input("Enter operator (+, -, *, /): ")

if operator == "+":
    result = num1 + num2
    print("Result =", result)

elif operator == "-":
    result = num1 - num2
    print("Result =", result)

elif operator == "*":
    result = num1 * num2
    print("Result =", result)

elif operator == "/":
    if num2 == 0:
        print("Error! Division by zero is not allowed.")
    else:
        result = num1 / num2
        print("Result =", result)

else:
    print("Invalid operator! Please use +, -, *, or /.")'''
    
    
    

print("===================================")
print("     WORD COUNTER & ANALYZER")
print("===================================")

paragraph = input("Enter a paragraph:\n")

words = paragraph.split()

word_count = len(words)

longest_word = ""

for word in words:
    if len(word) > len(longest_word):
        longest_word = word

vowels = "aeiouAEIOU"
vowel_count = 0

for char in paragraph:
    if char in vowels:
        vowel_count += 1

print("\n========== ANALYSIS ==========")
print("Total Words      :", word_count)
print("Longest Word     :", longest_word)
print("Length of Longest Word :", len(longest_word))
print("Total Vowels     :", vowel_count)
        
