# Collatz-with-try-and-excep-
def collatz(number):
    while number != 1:
        if number % 2 == 0:
            number = number // 2
            print(number)
        elif number % 2 != 0:
            number = number * 3 + 1
            print(number)


print("please put your number:")
try:
    num = int(input())
    collatz(num)
except ValueError:
    print("you put a non integer as an input")
