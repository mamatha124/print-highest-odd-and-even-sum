# print-highest-odd-and-even-sum in python
#to print the highest odd and even sum
#Approach-1
n=int(input())
a=list(map(int,input().split()))
e=0
o=0
for i in range(n):
  if a[i]%2==0 and a[i]>0:
    e=a[i]
  elif a[i]>o:
    o=a[i]
print(e+o)

#Approach-2
n=int(input())
a=list(map(int,input().split()))
e=0
o=0
for i in a:
  if i%2==0 and i>0:
    e=i
  elif i>o:
    o=i
print(e+o)

#Approach-3
n=int(input())
a=list(map(int,input().split()))
e=[]
o=[]
for i in range(n):
  if a[i]%2==0:
    e.append(a[i])
  else:
    o.append(a[i])
print(max(e)+max(o))

#Approach-4
n=int(input())
a=list(map(int,input().split()))
e=[]
o=[]
for i in a:
  if i%2==0:
    e.append(i)
  else:
    o.append(i)
print(max(e)+max(o))

