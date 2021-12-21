# test
test

from random import randrange 

def printLines(lis):
    for i in range(len(lis)):
            print(lis[i])
            
print(printLines([[1,2,3],[4,5],[6]]))

def sumListOfLists(lis):
    a = 0
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            a = a + lis[i][j]
    return a 

#print(sumListOfLists([[1,2,3],[4,5]]))


def holdOddInt(lis):
    a = False
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]%2!=0:
                a = True
    return False

#print(holdOddInt([[2, 4, 6], [8, 10], [12]]))

def numberOfDigigtInt(lis):
    a= 0
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]<=9:
                a = a + 1
    return a

#print(numberOfDigigtInt([[11, 3, 12], [1, 100]]))

def positionList(lis):
    l = []
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]%9==0:
                l = l + [True]
            else:
                l = l + [False]
    return l

#print(positionList([[9, 4, 27], [81], [3, 45]]))

def rowSums(lis):
    l = []
    for i in range(len(lis)):
        a = 0
        for j in range(len(lis[i])):
            a = a +lis[i][j]
        l = l + [a]
    return l
print(rowSums([[2, 3], [5, 8, 13, 21], [34]]))


def rowWiseCount(n,lis):
    l = []
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]>n:
                l = l + [i]
    return l
#print(rowWiseCount(10,[[12,1],[37, 8, -1, 21], [0]]))

#Exercice 3 :

def holddsCharlie(lis):
    a = False
    for i in  range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]=="Charlie":
                a = True
    return a

print(holddsCharlie(([["Riri", "Fifi", "Loulou"], ["Charlie", "Paul ", "Valéry"], ["Franz"]])))


def holdE(lis):
    a = False
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]=="e":
                a = True
    return a

print(holdE([["Il", "abandonna", "son", "roman", "sur", "son", " lit"], ["Il", "alla", "à", "son", "lavabo"]]))

def fWordPositions(a,lis):
    l =[]
    for i in range(len(lis)):
        for j in range(len(lis[i])):
            if lis[i][j]== a:
                l = l + [True]
            l = l + [False]
    return l

print(fWordPositions("son",[["Il", "abandonna", "son", "roman", " sur", "son", "lit"], ["Il", "alla", "à", "son", "lavabo"]]))
            
    
#Exercice 4 :

def squareOfZeros(n):
    l = [[0]*n]*n
    for i in range(n):
        for j in range(n):
            return l 
#print(squareOfZeros(3))

def rectOfInt(n,p):
    l = [[0]*p]*n
    for i in range(len(l)):
        for j in range(len(l[i])):
            l[i][j]=randrange(0,9)
    return l

#print(rectOfInt(3,2))
