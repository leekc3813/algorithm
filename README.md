## Algorithm

소스코드 블록은 다음과 같이 작성할 수 있습니다.

```py
n = int(input())

a=list(map(int,input().split()))
b=list(map(int,input().split()))

s = 0

for i in range(n):
  s += min(a) * max(b)
  a.pop(a.index(min(a)))
  b.pop(b.index(max(b)))

print(s)



```
