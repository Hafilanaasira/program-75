# program-75
# Initialize first two terms
a = 0
b = 1

# Read number of terms from user
n = int(input("Enter the number of terms in the sequence: "))

# Print the first two terms if n >= 1
if n <= 0:
    print("Please enter a positive integer")
elif n == 1:
    print(a)
else:
    print(a, b, end=" ")

    # Print remaining terms
    for _ in range(n - 2):
        c = a + b
        print(c, end=" ")
        a, b = b, c
Enter the number of terms in the sequence: 8
0 1 1 2 3 5 8 13
