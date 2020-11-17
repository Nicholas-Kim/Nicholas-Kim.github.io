---
title: "Python 여러가지 출력방법"
date: 2020-11-17
excerpt: "Python basic"
categories:
  - Python
tags:
  - print
  - python
  - computer language
  - end parameter
  - sep parameter
---

<p align="center">
<img src="https://cdn.pixabay.com/photo/2016/01/19/14/45/vintage-1148940_1280.jpg" width="700" height="350">
</p>

# print()

## 콤마 사용법
``` python
print('tmp1', 'tmp2')
```
> 실행결과
``` python
tmp1 tmp2
```
print문을 사용할 콤마를 사용하여 구분하면 한 칸 공백이 설정되어 띄어쓰기로 값을 구분해줍니다. 


## sep 파라미터 사용법
``` python
print('tmp1', 'tmp2', sep = ',')
print('tmp1', 'tmp2', sep = '__')
```
> 실행결과
```python
tmp1,tmp2
tmp1__tmp2
```
sep파라미터를 이용하게 되면 sep 파라미터에 지정된 값으로 구분자를 지정해줄 수 있습니다. 

## end 파라미터 사용법
python에서 기존의 print()문은 항상 엔터값이 포함되어있습니다. end 파라미터를 공백으로 처리하면 줄바꿈을 하지 않을 수 있습니다. 

```python
print('tmp1', end = ' ')
print('tmp2')
```
> 실행결과
```python
tmp1 tmp2
```

## join() 사용법
리스트를 출력할때는 join()을 이용할 수 있습니다. 
``` python
tmp_list = ['tmp1', 'tmp2']
print('(쓰고 싶은 구분자)'.join(tmp_list))
```
> 실행결과
``` python
tmp1 tmp2
```
join()앞 괄호에 쓰고싶은 구분자를 넣어 리스트를 묶어서 처리할 수 있습니다. 

## .foramt() 사용법
.format()을 사용하여 출력을 할수도 있습니다. 
```python
tmp = 0
name = "Kim"
print('{0}: {1}'.format(tmp+1, name)) #1번째 방법
print('{}: {}'.format(tmp+1, name)) #2번째 방법(인덱스 생략)
```
> 실행결과
```python
1: Kim
```

## f-string 사용법
```python
print(f'{tmp+1}:{name}')
```
> 실행결과
``` python
1: Kim
```

