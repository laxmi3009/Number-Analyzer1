# Number-Analyzer1

# Number Analyzer

num = int(input("Enter a number: "))

# Positive, Negative or Zero
if num > 0:
    print("Positive Number")
elif num < 0:
    print("Negative Number")
else:
    print("Zero")

# Even or Odd
if num % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")

# Prime or Not
if num < 2:
    print("Not a Prime Number")
else:
    prime = True

    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            prime = False
            break

    if prime:
        print("Prime Number")
    else:
        print("Not a Prime Number")

# Palindrome
if str(num) == str(num)[::-1]:
    print("Palindrome Number")
else:
    print("Not a Palindrome Number")