---
# page
title: "[OS#1] 프로세스 개념 정리"
excerpt: "컴퓨터를 이해해보기 - OS편"
layout : single
published: false
# classes: wide

# toc
toc: true
toc_sticky: true
toc_label: "목차"

# category & tag
categories:
  - OS
tags: 
  - OS, Process

# Time
read_time: true
date: 2021-11-08 
last_modified_at: 2021-11-08 
---

## :fire: 목표
> **1. 프로세스의 구성을 이해한다.**  

## :speech_balloon: 1. 프로세스의 구성

컴퓨터에서 일어나는 작업들을 이해하기 위해서는 프로세스에 대한 이해가 필요하다.  
우선 일반적인 전체 구조도 및 프로세스의 정의는 아래와 같다.

![프로세스](https://upload.wikimedia.org/wikipedia/commons/thumb/2/25/Concepts-_Program_vs._Process_vs._Thread.jpg/1280px-Concepts-_Program_vs._Process_vs._Thread.jpg)

> **프로세스는 컴퓨터의 메모리에서 실행 중에 있는 프로그램을 의미한다.**   
> **스케줄링의 TASK와 같은 의미로 쓰인다.**

**프로세스 구성**  

프로세스는 Code, Data, Heap, 메인스레드, 메인스레드 안에 Stack으로 이루어져 있다. (스레드는 나중에!)

| 항목 | 설명 |
| ------        | ----------- |
| Code          | 소스코드로 이루어진 프로그램을 구동하기 위해 소스코드를 저장해놓는 영역 |
| Data          | 전역 변수, 정적 변수, 배열 등과 관련된 데이터를 저장해놓는 영역 |
| Heap          | 동적 할당(new, malloc) 된 정보들이 저장하는 영역 |
| 메인스레드     | 기본적으로 프로세스는 최소 1개의 스레드(메인스레드)를 통해 프로세스 실행 |
| Stack         | 스레드 안에 위치, 지역 변수, 매개 변수, 함수, 함수 리턴 값 등 임시 메모리 영역 |

※ 여담이지만 Docker 컨테이너도 리눅스 프로세스와 chroot 기반으로 동작한다고 한다. [참고자료](https://www.44bits.io/ko/post/change-root-directory-by-using-chroot)


## :memo: 결론

> **프로세스 구성 : CODE, DATA, HEAP, 메인스레드, STACK**  
> **프로세스 라이프사이클 : 생성, 실행, 준비, 대기, 종료**  
> **프로세스 간 통신 방법 : 공유 메모리, 메시지 패싱**  

## :question: 추후 공부할 것



