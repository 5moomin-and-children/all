# 내가 분리수거 왕이 될 상인가

Sparta Coding Camp - Team Project 2. AI classification project

*자세한건 wiki에 적혀있습니다!

<br>
<br>

## 😎 5조 무민과 아이들
* [윤소현님](https://github.com/YoonSeohyeon) (팀장)
* [이병준님](https://github.com/dugadak)
* [한장원님](https://github.com/HANJANGWON)
* [이용헌님](https://github.com/yongheon-Lee)
* [박재영님](https://github.com/devjcode)

<br>
<br>

## ☁️개발 포지션
+ CTO : 윤소현
+ Front-end : 박재영, 윤소현
+ Back-end : 윤소현, 이용헌
+ AI : 한장원, 이병준

<br>
<br>

## 📆프로젝트 기간
2022-01.12 ~ 2022-01.18

<br>
<br>

## 🤖 기술 스택
1. Front : HTML, JavaScript, Ajax
2. Back : Python, Flask, MongoDB
3. AI : Google Colab, tensorflow
4. 협업 : [github](https://github.com/MoominAndChildrenTeam/), [Figma](https://www.figma.com/file/bxfXRmb2SybXbWdoB3PudW/%EB%AC%B4%EB%AF%BC?node-id=0%3A1)

<br>
<br>

## 🕸 아키텍처
![image](https://user-images.githubusercontent.com/56148289/149078041-f5da0cd8-f796-473c-80b0-d0aca7015de8.png)

## 🙉 구현
- 로그인
- 회원가입
- recycle 페이지
  + 업로드된 이미지 분류 후 점수 반영
- result 페이지
  + 분리수거 점수 랭킹 표시
  
  <br>
<br>

## 🎈 DB 스키마  
|기능|method|url|request|response|
|---|---|---|---|---|
|로그인 기능|GET|/api/login|{'id':id,'pw':'pw'}|/index.html {True(토큰), False}|
|회원가입 기능|GET|/sign_up|.|회원가입 페이지 로드|
|.|POST|/api/sign_up|{'id':id,'pw':'pw'}|sign_up{token}|
|분리수거 기능|GET|/recycle|.|recycle 페이지 로드|
|.|POST|/api/recycle_check|{'trash_image':trash_image}|url:recycle{True/False}|
|분리수거 제출기능|POST|/api/submit|{'id':id,'score':score}|url:result{ranking list}|
|결과|GET|/result|.|result 페이지 로드|
