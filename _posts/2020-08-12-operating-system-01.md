---
layout: post
title: "[OS]1. Operating System Overview"
tags: [운영체제, OS]
comments: true
---

운영체제 정리 첫 번째 글,<br/>
Overview

---

## 1. Operating System Overview

### 운영체제란?

컴퓨터 시스템의 자원들을 효율적으로 관리하며, 사용자가 컴퓨터를 편리하고 효과적으로 사용할 수 있도록 환경을 제공하는 <mark>소프트웨어</mark>

#### Key Interfaces

* Instruction Set Architecture(ISA)
    * 컴퓨터가 따를 수 있는 언어 instruction
    * 하드웨어와 소프트웨어 사이의 경계 인터페이스
* Application Binary Interface(ABI)
    * 프로그램간 휴대성을 위함
    * System call Interface를 정의
    * System Call: OS에게 프로그램이 해야할 일을 말하는 것
* Application programming Interface(API)
    * High-level language 라이브러리

#### Kernel
메인 메모리에 들어가 있는 Operating System - OS의 핵심적인 부분<br/>
Program과 Data의 양이 많이 들어갈 수 있도록 OS의 핵심적 기능만 메인 메모리에 적재

#### Programming 종류
##### 1. Uni-programming

<img src="../images/20200812-os-01/Uni-programming.png" alt="Uni-programming"  style="width:600px;height:auto;"/>
프로세서(CPU)는 I/O가 종료될 때 까지 기다림. 한번에 한가지 프로그램만 실행

##### 2. Multi-programming
<img src="../images/20200812-os-01/Multi-programming.png" alt="Multi-programming"  style="width:600px;height:auto;"/>
I/O interrupt 발생 시 다른 Job으로 Switch하여 실행 <br/>

* 장점: CPU가 기다리는 시간이 줄어듦
* 단점: 큰 메모리 공간 필요

