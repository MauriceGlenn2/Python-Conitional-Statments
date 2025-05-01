# Python-Conitional-Statments

# 🎢 Rollercoaster Ride Eligibility & Billing

## 🧠 What I Learned
In this mini-project, I learned the importance and power of **conditional statements** in Python. I practiced using `if`, `elif`, and `else` to guide the flow of logic based on user input. I also used `input()`, type casting, and basic arithmetic to simulate a simple billing system.

## 📜 What the Code Does
This script simulates a rollercoaster ticket booth system:
- It checks if a person is tall enough (120 cm or more) to ride.
- If eligible, it calculates the ticket price based on age:
  - Kids (≤12): $5
  - Teens (13–18): $7
  - Adults (>18): $12
- It adds $3 to the bill if the rider wants a photo.
- Finally, it prints the total bill.
- If the rider is too short, it displays a friendly rejection message.

## 💻 Code

```python
print("Welcome to the rollercoaster!")
height = int(input("What is your height in cm? "))
bill = round(0, 2)

if height >= 120:
    print("You can ride the rollercoaster")
    age = int(input("What is your age? "))
    if age <= 12:
        bill = 5
        print(f"Kids 12 tickets are ${bill}")
    elif age <= 18:
        bill = 7
        print(f"Ages 12 to 18 tickets are ${bill}")
    else:
        bill = 12
        print(f"Adult tickets are ${bill}")

    want_photo_taken = input("Do you want your photo taken? Type n for No and y for Yes ")
    if want_photo_taken == "y":
        bill += 3
    print(f"Your final bill is ${bill}")
else:
    print("Sorry you have to grow taller before you can ride.")

