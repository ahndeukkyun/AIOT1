# 파이썬 기본 문법 정리

## 1. 변수와 자료형

```python
x = 10        # 정수
y = 3.14      # 실수
name = "Alice"  # 문자열
is_ok = True    # 불린
```

## 2. 주석

- 한 줄 주석: `#` 사용
- 여러 줄 주석처럼 사용하려면 `'''` 또는 `"""` 문자열을 활용

```python
# 이것은 한 줄 주석입니다.

'''
이것은 여러 줄 주석처럼 사용되는 문자열입니다.
'''
```

## 3. 출력과 입력

```python
print("Hello, world!")  # 출력
name = input("이름을 입력하세요: ")  # 입력
```

## 4. 연산자

```python
# 산술 연산
a + b, a - b, a * b, a / b, a // b, a % b, a ** b

# 비교 연산
a == b, a != b, a > b, a < b, a >= b, a <= b

# 논리 연산
and, or, not
```

## 5. 조건문

```python
if score >= 90:
    print("A")
elif score >= 80:
    print("B")
else:
    print("F")
```

## 6. 반복문

```python
# while 반복문
i = 0
while i < 5:
    print(i)
    i += 1

# for 반복문
for i in range(5):  # 0부터 4까지
    print(i)
```

## 7. 리스트, 튜플, 딕셔너리

```python
# 리스트
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits[1])  # banana

# 튜플 (수정 불가)
t = (1, 2, 3)

# 딕셔너리
person = {"name": "Tom", "age": 20}
print(person["name"])  # Tom
```

## 8. 함수 정의

```python
def add(a, b):
    return a + b

print(add(3, 5))  # 8
```

## 9. 클래스

```python
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, I'm {self.name}")

p = Person("Alice")
p.greet()
```

## 10. 예외 처리

```python
try:
    x = int(input("숫자 입력: "))
    print(10 / x)
except ZeroDivisionError:
    print("0으로 나눌 수 없습니다.")
except ValueError:
    print("숫자가 아닙니다.")
finally:
    print("프로그램 종료")
```
