https://school.programmers.co.kr/learn/courses/30/lessons/120907

23/02/19

---

나는 저렇게 비교하는 방식으로 풀었는데 다른 사람이 푼 코드를 보니까 훨씬 간단한 법이 있었다...

```python
def valid(equation):
    equation = equation.replace('=', '==')
    return eval(equation)

def solution(equations):
    return ["O" if valid(equation) else "X" for equation in equations]
```

`eval` 함수를 몰랐음...
현업에서는 쓰면 안된다지만 eval을 사용하면 간단하게 해결할 수 있는 문제였다.

파이썬 내장함수 더 공부하기..
