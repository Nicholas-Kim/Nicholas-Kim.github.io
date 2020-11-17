---
title: "Python Enumerate"
date: 2020-11-15 01:09:11
excerpt: "Python basic"
categories:
  - Python
tags:
  - Enumerate
  - python
  - computer language
---

<p align="center">
<img src="https://cdn.pixabay.com/photo/2016/02/18/14/42/syndicate-1207270_960_720.jpg" width="400" height="150">
</p>

## enumerate()
Enumerate는 '열거하다'는 뜻의 함수이다. enumerate함수는 iteration한 자료형을 index와 value를 tuple형태로 리턴합니다. 


``` python
test_list = [1, 10, 2, 3, 5]
print(list(enumerate(test_list)))
```
이 코드를 실행하게 되면
``` python
[(0, 1), (1, 10), (2, 2), (3, 3), (4, 5)]
```
이와 같이 tuple 형태로 index와 value를 같이 리턴해줍니다.



## enumerate() for문에서의 활용

enumerate는 for문에서도 사용이 가능합니다.
```python
for i, v in enumerate(test_list):
    print(i, v)
```

```python
0 1
1 10
2 2
3 3
4 5
```

이렇게 사용하면 index와 value 모두 깔끔하게 처리할 수 있습니다. 
