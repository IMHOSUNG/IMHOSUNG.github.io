---
# page
title: "약수의 개수와 덧셈"
excerpt: "알골리즘 공부"
layout : single
published: true
# classes: wide

# toc
toc: true
toc_sticky: true
toc_label: "목차"

# category & tag
categories:
  - algorithm
tags: 
  - Level1

# Time
read_time: true
date: 2021-11-11 
last_modified_at: 2021-11-11 
---

## :fire: 문제 이해
 1. 별 달리 이해할 것 없음

## :speech_balloon: 로직

 1. 약수 구하기
 2. 갯수 가지고 처리하기

## :speech_balloon: 코드

``` python
def solution(left, right):
    answer = 0
    
    for num in range(left,right+1):
        count = 0
        for i in range(1,num+1):
            if(num%i==0):
                count+=1
        
        if count%2==0:
            answer+=num
        else:
            answer-=num
    
    return answer
```

## :memo: 결론
 1. 레벨 1부터 파이썬 익숙해지고 차근 차근 풀어보자


