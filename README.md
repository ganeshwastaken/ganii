lower = int(input("lower: "))
upper = int(input("upper: "))
c=[]
b=[]

for num in range(lower, upper + 1):

    # all prime numbers are greater than 1
    if num > 1:

        for i in range(2, num):
            if (num % i) == 0:
                print("Composite number", num)
                c.append(num)
                break
        else:
            b.append(num)
            print("Prime number", num)
print("count for prime numbers:",c)
print("count for composite numbers:",b)
