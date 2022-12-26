---
title: "알고리즘 분석"
excerpt: "시간복잡도, 공간복잡도, 빅오표기법"

categories:
  - Algorithm
tags:
  - [시간복잡도, 공간복잡도, 빅오표기법]

permalink: /categories5/알고리즘1/

toc: true
toc_sticky: true

date: 2022-12-26
last_modified_at: 2022-12-26
---

## 알고리즘 분석

- ### 공간 복잡도(Space Complexity)
  - 알고리즘이 문제 해결시 차지하는 메모리등의 공간을 뜻한다.

- ### 시간 복잡도(Time Complexity)
  - 알고리즘이 문제 해결시 처리하는데 소요되는 시간을 뜻한다.
  - 방법
    - 실제적 방법
      - 입출력 데이터 양이 알고리즘에 미치는 여향을 직접 관찰 및 기록하는 방법이다.
      - 정확성이 낮고 사용 범위가 제한적이다.
    - 수학적 방법
      - 알고리즘의 성능이 최악이되는 경계를 알고, 평균 성능을 계산하여 구하는 방법이다.
      - 빅오표기법을 주로 사용한다.

- ### 빅오 표기법(Big-O)
  - 빅오의 O는 Order(지수) of complexity의 O이다.
  - 표기 방식 (성능이 좋은 순으로 나열)
    - O(1)
    - O(n)
    - O(log n)
    - O(n log n)
    - O(n^2)
    - O(2^n)
    - O(n!)