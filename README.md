

print("---------calculator--------")
import math
print("1. Addition")
print("2. Subtraction")
print("3. Multiply")
print("4. Divide")
print("5. Square Root")
print("6. Power")
choice = int(input("Enter the choice (1 , 2 , 3 , 4 , 5 , 6) : "))
if choice in [1 , 2 , 3 , 4 , 6]:
    a = float(input("Enter the first value : "))
    b = float(input("Enter the second value : "))
    if choice == 1:
        print("Result =", a + b)
    elif choice == 2:
        print("Result =", a - b)
    elif choice == 3:
        print("Result =", a * b)
    elif choice == 4:
        if b != 0:
            print("Result =", a / b)
        else:
            print("Error 'Division by 0'")
    elif choice == 6:
        print("Result =", math.pow(a , b))
elif choice == 5:
    num = float(input("Enter the value : "))
    print("Result =", math.sqrt(num))
else:
    print("Invalid Number")
