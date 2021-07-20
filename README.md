# python_learning

from : https://pydole.tistory.com/entry/Python-sort-reverse%EC%99%80-sorted-reversed-%EC%B0%A8%EC%9D%B4

sorted : iterator의 요소를 정렬하여 리턴 하지만 원본은 변경하지 않는다. (파이썬 내장함수)

reversed : iterator의 요소를 역순으로 리턴 하지만 원본은 변경하지 않는다. (파이썬 내장함수)

list.sort() list.reverse() 원본을 변경하지만 리턴 값은 None

```python
import random

Numbers = random.sample([ i for i in range(1,20,1)],6)

print(sorted(Numbers))    # 정렬하여 리턴 하지만 원본은 변경하지 않는다.
print(Numbers)            # 원본은 변경되지 않았음.

Numbers.sort()            # [].sort  원본 자체를 정렬하지만 리턴은 None
print(Numbers)

-----------------------------------------------------------------------

[3, 4, 5, 6, 7, 14]
[14, 6, 5, 7, 4, 3]
[3, 4, 5, 6, 7, 14]


lst = [ i for i in range(5)]
print(list(reversed(lst))) # reversed
print(lst) # original
--------------------------------------------
[4, 3, 2, 1, 0]
[0, 1, 2, 3, 4] 
```
