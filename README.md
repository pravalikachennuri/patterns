this file contains some of the patterns in python language
# pattern 1

def pattern_1(n):
    for i in range(n):
        for j in range(n):
            print("*",end=' ')
        print()
n=int(input('enter : '))
pattern_1(n)

# pattern 2

def pattern_2(n):
    for i in range(1,n+1):
        for j in range(i):
            print('*',end=' ')
        print()
n=int(input('enter : '))
pattern_2(n)

# pattern 3

def pattern_3(n):
    for i in range(1,n+1):
        for j in range(1,n+1):
            print(j,end=' ')    
        print()
n=int(input('enter : '))
pattern_3(n)

# pattern 4

def pattern_4(n):
    for i in range(1,n+1):
        for j in range(i):
            print(i,end=' ')
        print()
n=int(input('enter : '))
pattern_4(n)
 
# pattern 5

def pattern_5(n):
    for i in range(n):
        for j in range(n,i,-1):
            print("*",end=' ')
        print()
n=int(input('enter : '))
pattern_5(n)

# pattern 6

def pattern_6(n):
    for i in range(n,0,-1):
        for j in range(i):
            print(j,end=' ')
        print()
n=int(input('enter : '))
pattern_6(n)

# pattern 7

def pattern_7(n):
    for i in range(n):
        for j in range(n,i,-1):
            print(j,end=' ')
        print()
n=int(input('enter : '))
pattern_7(n)

# pattern 8

def pattern_8(n):
    for i in range(n):
        for j in range(n-i-1):
            print(" ",end=" ")
        for k in range(2*i+1):
            print("*",end=' ')
        for l in range(n-i-1):
            print(" ",end=' ')
        print()
n=int(input('enter : '))
pattern_8(n)

# pattern 9

def pattern_9(n):
    for i in range(n):
        for j in range(i):
            print(' ',end=' ')
        for k in range(2*n-(2*i+1)):
            print('*',end=" ")
        for l in range(i):
            print(' ',end=' ')
        print()
n=int(input('enter : '))
pattern_9(n)

# pattern 10

def pattern_10(n):
    pattern_8(n)
    pattern_9(n)
n=int(input("enter : "))
pattern_10(n)

# pattern 11

def pattern_11(n):
    for i in range(1,2*n):
        if i>n:
            for j in range(2*n-i):
                print("*",end=" ")
            print()
        else:    
            for k in range(i):
                print("*",end=" ")
            print()
n=int(input("enter : "))
pattern_11(n)

# pattern 12

def pattern_12(n):
    start=1
    for i in range(1,n+1):
        if i%2==0:
            start=1
        else:
            start=0
        for j in range(i):
            print(start,end=" ")
            start=1-start
        print()
n=int(input("enter : "))
pattern_12(n)    

# pattern 13

def pattern_13(n):
    spaces=2*(n-1)
    for i in range(1,n+1):
        for j in range(1,i+1):
            print(j,end=" ")
        for k in range(spaces):
            print(" ",end=" ")
        for l in range(i,0,-1):
            print(l,end=" ")
        print()
        spaces-=2
n=int(input("enter no. :"))
pattern_13(n)

# pattern 14

def pattern_14(n):
    num=1
    for i in range(1,n+1):
        for j in range(i):
            print(num,end=' ')
            num+=1
        print()
n=int(input("enter : "))
pattern_14(n)

# pattern 15

def pattern_15(n):
    for i in range(1,n+1):
        for j in range(i):
            print(chr(j+65),end=" ")
        print()
n=int(input("enter : "))
pattern_15(n)

# pattern 16

def pattern_16(n):
    for i in range(n,0,-1):
        for j in range(i):
            print(chr(j+65),end=" ")
        print()
n=int(input("enter : "))
pattern_16(n)

# pattern 17

def pattern_17(n):
    for i in range(1,n+1):
        for j in range(i):
            print(chr(i+64),end=" ")
        print()
n=int(input("enter : "))
pattern_17(n)

# pattern 18

def pattern_18(n):
    for i in range(1,n+1):
        #spaces
        for j in range(n-i):
            print(" ",end=" ")
        # aplabets
        for k in range(2*i-1):
            print(chr(k+65),end=' ')
        #spaces
        for j in range(n-i):
            print(" ",end=" ")
        print()
n=int(input("enter : "))
pattern_18(n)

# pattern 19

def pattern_19(n):
    for i in range(1,n+1):
        for j in range(i,0,-1):
            print(chr((n-j)+65),end=' ')
        print()
n=int(input("enter : "))
pattern_19(n)

# pattern 20

def pattern_20(n):
    spaces=0
    for i in range(n):
        for o in range(n-i):
            print("*",end=" ")
        for p in range(spaces):
            print(" ",end=" ")
        for q in range(n-i):
            print('*',end=" ")
        print()
        spaces+=2
    spaces=2*(n-1)
    for m in range(1,n+1):
        for j in range(m):
            print("*",end=' ')
        for k in range(spaces):
            print(" ",end=" ")
        for l in range(m):
            print("*",end=" ")
        print()
        spaces-=2
n=int(input("enter : "))
pattern_20(n)

# pattern 21

def pattern_21(n):
    spaces=2*(n-1)
    for i in range(1,2*n):
        if i<n:
            for j in range(i):
                print("*",end=' ')
            for k in range(spaces):
                print(" ",end=" ")
            for l in range(i):
                print("*",end=" ")
            print()
            spaces-=2
        else:
            for m in range((2*n)-i):
                print("*",end=" ")
            for r in range(spaces):
                print(" ",end=" ")
            for v in range((2*n)-i):
                print("*",end=" ")
            print()
            spaces+=2

n=int(input("enter : "))
pattern_21(n)

# pattern 22

def pattern_22(n):
    for i in range(n):
        for j in range(n):
            if (j==0) or (j==n-1) or (i==0) or (i==n-1):
                print("*",end=' ')
            else:
                print(" ",end=' ')
        print()
n=int(input("enter : "))
pattern_22(n)

# pattern 23

def pattern_23(n):
    for i in range(2*n-1):
        for j in range(2*n-1):
            top=i
            left=j
            right=(2*n-2)-i
            bottom=(2*n-2)-j
            print(n-min(min(top,bottom),min(left,right)),end=' ')
        print()
n=int(input("enter : "))
pattern_23(n)
