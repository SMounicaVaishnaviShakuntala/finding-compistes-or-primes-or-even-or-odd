# finding-compistes-or-primes-or-even-or-odd
import random
def prime(x):
    for i in range(2,x):
        if x%i==0:
            return False
    return True
a=float(input('Enter lower limit: '))
b=float(input('Enter upper limit: '))
x=random.randint(a,b)
print("\n")
print("Range is (%d,%d) and randomly picked number is %d"%(a,b,x))
if x>=0:
    print('%d is positive number'%(x))
    if x%2==0:
        print('%d is even number'%(x))
    else:
        print('%d is odd number'%(x))
    if prime(x)and x!=1 and x!=0:
        print('%d is prime number'%(x))
    elif prime(x) and x==1 or x==0:
        print('%d is neither a prime nor a composite number'%(x))
        
    else:
        print('%d is composite number'%(x))
else:
    print('%d is negative number'%(x))
    if x%2==0:
        print('%d is even number'%(x))
    else:
        print('%d is odd number'%(x))
    print('Negative numbers are neither prime nor composite numbers')
23
