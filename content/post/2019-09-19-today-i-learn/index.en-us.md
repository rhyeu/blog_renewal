---
title: Today I Learn / python tip (print, list, 계산)
author: 류성균
date: '2019-09-19'
slug: index.en-us
categories:
  - Today I learn
tags:
  - python
  - python list
  - computing
keywords:
  - tech
---

<!--more-->



- 요새 코드업 기초 100제를 풀어보고 있는데 헷갈리는 것들을 정리!

# 1. sep 옵션 in python

파이썬에서 여러 개를 출력할 때 sep 옵션을 걸 수 있음

```
print(1920, 1080, sep = 'x')
print('Hello', 'Python', sep = '-')
```

# 리스트 원소 합치기
- 출처 : http://mwultong.blogspot.com/2006/12/python-list-merge.html
```
PA = ["pine", "apple"]

## 그냥 합치기
value = "".join(PA)
print(value)

## 구분자를 넣어 합치기
value2 = ", ".join(PA)
print(value2)
```


# 진법 변환
- 출처 : https://www.daleseo.com/python-int-bases/
```
## 10진법 -> 다른 진법
format(50, 'b') # 이진법
format(50, 'o') # 8진법
format(50, 'x') # 16진법 (소문자)
format(50, 'X') # 16진법 (대문자)
format(50, 'X') # 16진법 (대문자)
```

```
## 다른 진법 -> 10진법
format(int('2A', 16), 'd')
format(int('62', 8), 'd')
```

```
### 다른 진법 -> 다른 진법
format(int('2A', 16), 'o')
format(int('62', 8), 'X')
```

# 항상 헷갈리는 몫과 나머지
- 참조 : https://programmers.co.kr/learn/courses/4008/lessons/12732
```
a = 4; b = 7

print(a//b) # 몫
print(a%b) # 나머지
```

# 아스키 코드 <-> 문자열
```
print(ord('B')) # 문자를 아스키 코드로 변환
print(chr(102)) # 아스키코드를 문자로 변환
```

# 리스트의 문자열을 int 형태로 변환
```
a = ['13', '4', '68']

a1 = list(map(int, a)) # 맵핑을 이용한 방법
print(a1)
a2 = [int(i) for i in a] # 리스트 컴프리헨션을 이용한 방법
print(a2)
```



### 괄호 없이 리스트 출력하기

리스트

```
a = [1,2,'X',4,5]

print(*a, sep = " ")
```

### 파이썬 비트 연산자

- AND : &
- OR : |
- XOR : ^
- NOT : ~

### 삼항 연산자
- 익숙해지면 코드가 더 간단해 질듯

```
a = 10
b = 16

print(a if a>b else b)
```

### 파이썬 range 함수

range 함수는 파이썬 슬라이싱 처럼 range의 두번째 파라미터 앞에서 끊긶다.
```
for i in range(1,9):
  print(i)
```

