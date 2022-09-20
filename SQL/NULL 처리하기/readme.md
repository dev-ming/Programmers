https://school.programmers.co.kr/learn/courses/30/lessons/59410

2022/09/20

<br>

## MySQL NULL값 처리

---

### IFNULL

해당 column의 값이 NULL을 반환할 때, 다른 값으로 출력할 수 있도록 해주는 함수

<br>

- 기본구조

```sql
IFNULL(Column,"NULL일 때 출력되는 값")
```

- 사용 예시 (문제)

```sql
//NAME이 NULL인 경우 No name 으로 출력
SELECT ANIMAL_TYPE,
IFNULL(NAME,"No name") as NAME
```

<br>

### NVL()

오라클에서 사용하는 함수

NULL 값인 경우 특정값으로 출력하고 싶을 때는 **NVL** 함수 사용

NULL 값이 아닌 경우 특정값으로 출력하고 싶을 때는 **NVL2** 함수 사용

<br>

- 기본구조

```sql
//NULL인 경우 지정값 출력, 아닌 경우 원래 값 출력
NVL("값","지정값")

//NULL이 아닌 경우 지정값1 출력, NULL인 경우 지정값2 출력
NVL2("값","지정값1","지정값2")
NVL2("값","NOT NULL","NULL")
```
