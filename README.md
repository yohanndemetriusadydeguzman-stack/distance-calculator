# Reflection:
# Using a library is more practical because it provides reliable, optimized 
# tools that prevent us from having to recreate complex math algorithms. 
# For example, using math.sqrt() lets us instantly find the square root 
# without wasting time writing an entire approximation loop from scratch.

import math

print("--- 2D Distance Calculator ---")

try:
    # Get user coordinates safely
    x1 = float(input("Enter x1: "))
    y1 = float(input("Enter y1: "))
    x2 = float(input("Enter x2: "))
    y2 = float(input("Enter y2: "))

    # Calculate distance using math.pow (or the simpler ** operator)
    # Formula: d = √((x2-x1)² + (y2-y1)²)
    distance = math.sqrt(math.pow(x2 - x1, 2) + math.pow(y2 - y1, 2))

    # Display result rounded to two decimal places
    print(f"\nThe distance between the two points is: {distance:.2f}")

except ValueError:
    print("\nError: Please enter numbers only. Letters and symbols are not allowed.")

