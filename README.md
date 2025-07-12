# Training
#01 Minimum overtime payment 
n=int(input())
m=list(map(int,input().split()))
d=list(map(int,input().split()))
x=int(input())
m.sort()
d.sort(reverse=True)
c=0
for i in range(n):
  if m[i]+d[i]>x:
    c=c+(m[i]+d[i]-x)
print(c*100)
