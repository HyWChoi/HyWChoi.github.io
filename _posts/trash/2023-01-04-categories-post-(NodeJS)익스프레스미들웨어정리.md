---
title: "[NodeJS] 익스프레스 미들웨어 정리"
excerpt: "middleware"

categories:
  - trash
tags:
  - [middleware]

permalink: /categories/trash

toc: true
toc_sticky: true

date: 2023-01-04
last_modified_at: 2022-01-04
---

익스프레스는 미들웨어가 핵심이다.

## 미들웨어란?

- 요청과 응답 사이에 위치해있다.
- 라우터와 에러 핸들러 등이 미들웨어이다.
- app.use를 통해 사용한다.
- **_실행 방법_**
  - app.use(middleware) -> 모든 요청에서 미들웨어가 실행
  - app.use('/about', middleware) -> /about을 포함한 하위 경로등에서 모두 실행
  - app.get('/about', middleware) -> /about으로 시작하는 post에서 middleware 실행
  - **app.use VS app.get**
    - use의 경우 /about, /about:id 등 모두 실행
    - get의 경우 /about 과 정확히 일치할 때만 실행
- 에러처리 미들웨어
  - (err,req,res,next)를 받음
  - 예외적인 경우를 제외한 모든 경우 최하단에 에러처리 미들웨어를 위치 시킴
  - err에는 에러에 대한 정보가 담긴다.

## 자주 사용하는 미들웨어 정리

### morgan
