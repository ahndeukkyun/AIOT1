# Numpy 기본 문법

## 1. Numpy 설치

Numpy는 Python에서 기본적으로 제공되지 않기 때문에 먼저 설치해야 합니다. 아래와 같이 `pip` 명령어를 사용하여 설치할 수 있습니다.

```bash
pip install numpy
```

## 2. Numpy 임포트

```python
import numpy as np
```

`np`는 Numpy를 사용할 때 자주 사용하는 별칭입니다.

## 3. Numpy 배열 (Array)

Numpy의 가장 기본적인 객체는 **배열**입니다. 배열은 리스트와 비슷하지만 더 효율적이고, 벡터화 연산이 가능합니다.

### 배열 생성

- **리스트를 배열로 변환**

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr)
```

- **다차원 배열 생성**

```python
arr_2d = np.array([[1, 2], [3, 4], [5, 6]])
print(arr_2d)
```

### 배열의 속성

```python
print(arr.shape)   # 배열의 차원
print(arr.ndim)    # 배열의 차원 수
print(arr.size)    # 배열의 전체 요소 개수
print(arr.dtype)   # 배열의 데이터 타입
```

## 4. Numpy 배열의 기본 연산

- **배열 덧셈과 뺄셈**

```python
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])

# 배열 덧셈
result_add = arr1 + arr2
print(result_add)

# 배열 뺄셈
result_sub = arr1 - arr2
print(result_sub)
```

- **배열 곱셈과 나눗셈**

```python
result_mul = arr1 * arr2
print(result_mul)

result_div = arr1 / arr2
print(result_div)
```

## 5. Numpy의 유용한 함수들

- **배열 생성 함수들**

```python
# 0으로 채운 배열
arr_zeros = np.zeros((3, 4))
print(arr_zeros)

# 1로 채운 배열
arr_ones = np.ones((2, 3))
print(arr_ones)

# 주어진 범위의 값을 갖는 배열
arr_range = np.arange(0, 10, 2)
print(arr_range)

# 균일한 간격으로 나누어진 배열
arr_linspace = np.linspace(0, 1, 5)
print(arr_linspace)
```

- **배열의 통계적 연산**

```python
arr = np.array([1, 2, 3, 4, 5])

# 평균
print(np.mean(arr))

# 표준편차
print(np.std(arr))

# 합
print(np.sum(arr))

# 최소값, 최대값
print(np.min(arr), np.max(arr))
```

- **배열의 조건 필터링**

```python
arr = np.array([1, 2, 3, 4, 5])

# 배열에서 3보다 큰 값만 선택
result = arr[arr > 3]
print(result)
```

## 6. 다차원 배열 (2D, 3D)

- **배열 슬라이싱 (2D 배열)**

```python
arr_2d = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])

# 2D 배열에서 첫 번째 행과 두 번째 행을 선택
print(arr_2d[0, :])   # 첫 번째 행
print(arr_2d[:, 1])    # 두 번째 열
```

- **배열 합치기와 나누기**

```python
arr1 = np.array([[1, 2], [3, 4]])
arr2 = np.array([[5, 6], [7, 8]])

# 수평 결합 (수평 스택)
arr_hstack = np.hstack((arr1, arr2))
print(arr_hstack)

# 수직 결합 (수직 스택)
arr_vstack = np.vstack((arr1, arr2))
print(arr_vstack)
```

## 7. Numpy의 선형 대수 함수

- **행렬 곱셈**

```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

result = np.dot(A, B)
print(result)
```

- **역행렬 구하기**

```python
A_inv = np.linalg.inv(A)
print(A_inv)
```

## 8. 난수 생성

```python
# 0과 1 사이의 난수 생성
random_arr = np.random.rand(3, 4)
print(random_arr)

# 정수 범위 내 난수 생성
random_int_arr = np.random.randint(0, 10, size=(2, 3))
print(random_int_arr)
```

