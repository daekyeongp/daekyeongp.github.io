---
title: Github 나만의 프로필(Profile) 만들기 🧑‍🎓
date: '2022-03-26 00:5:00 +0900'
categories: [Git & Github] # categories: [TOP_CATEGORIE, SUB_CATEGORIE]
tags: [Github, Profile]     # TAG names should always be lowercase
---

![profile](https://images.velog.io/images/daekyeong/post/5d7ea480-f74b-4e08-a911-fc68ffea2cd0/image.png)

---

# 1. Github Repository 생성👏
* 프로필용 **Github Repository**를 생성하는데 **github**에서 아래와 같이 설명하고 있다.

> * GitHub will display your profile README on your profile page if **all of the following are true.**
  1. You've created a repository with a **name that matches your GitHub username.**
  2. The repository is **public.**
  3. The repository **contains a file named README.md in its root.**
  4. The **README.md** file contains any content.

* 즉, **Repository** 이름을 내 **github** 아이디와 같게 생성하고 **Repository를 public**으로 설정하면 된다.

![repository](https://images.velog.io/images/daekyeong/post/d8b55985-3e1e-45a7-85bb-8ef92de2eaac/image.png)

* 위의 그림과 같이 **설정**하고 **Repository**를 생성하면 `README.md` 파일이 생성된다.

## TIP👍
* `README.md` 파일을 편집할 때 아래의 그림과 같이 코드를 작성하는 화면이 나온다.

![editfile](https://images.velog.io/images/daekyeong/post/a9c1e237-c3d6-42c2-bdf3-68e922af02bb/image.png)

* `Edit file` 오른쪽에 `Preview`를 누르면 `Commit`을 하기 전에 **미리보기**가 가능하다.

* 하지만, 이조차도 왔다갔다 너무 **귀찮다..**
그래서 찾아본 결과 [dillinger](https://dillinger.io/) 사이트를 이용하면 **작성한 Markdown 코드의 결과를 바로 확인할 수 있다.**

![dillinger](https://images.velog.io/images/daekyeong/post/738eb3ac-0e01-42e0-9d1c-f0c9791e2098/image.png)

# 2. 프로필 만들기
## 2.1 Capsule render
![header](https://capsule-render.vercel.app/api?type=waving&color=0:a82da8,100:da8f00&height=230&section=header&text=DaeKyeongPark&fontAlign=70&fontAlignY=40&fontSize=60&fontColor=ffffff)
* 사용 방법은 매우 간단하다.
```Javascript
![header](https://capsule-render.vercel.app/api?type={원하는 타입}&color={원하는 색상}&height={이미지 크기}&section={배경 이미지 타입}&text={텍스트 내용}&fontSize={폰트 크기})

// 내가 사용한 코드
![header](https://capsule-render.vercel.app/api?type=waving&color=0:a82da8,100:da8f00&height=230&section=header&text=DaeKyeongPark&fontAlign=70&fontAlignY=40&fontSize=60&fontColor=ffffff)
```

👉 출처 : https://github.com/kyechan99/capsule-render

## 2.2 배지 & 아이콘 사용하기
* 아래의 그림처럼 다른 블로그 처럼 **배지**로 멋있게 정리하고 싶었다.

![shields](https://images.velog.io/images/daekyeong/post/a1f738a2-141b-4f05-83eb-87473bc73f51/image.png)

* **배지** https://shields.io/
* **아이콘** https://simpleicons.org/
* 위의 링크를 통해 원하는 **배지와 아이콘**을 사용할 수 있다.
* 내가 사용한 **Javascript**의 코드는 다음과 같다.

```Javascript
<img src="https://img.shields.io/badge/Javascript-ffb13b?style=flat-square&logo=javascript&logoColor=white"/></a>&nbsp
```

* 위의 코드만 보면 햇갈릴 수 있는데 쉽게 설명하면 다음과 같다.

```Javascript
<img src="https://img.shields.io/badge/{사용할 텍스트-simpleicons 코드}style=flat-square&logo={simpleicons 아이콘이름}&logoColor=white"/></a>&nbsp
```
* `Tech Blog`, `Gmail`과 같이 링크를 걸기위해선 `a 태그`를 이용하면 된다.

```javascript
<a href="{링크 주소}"><img src="https://img.shields.io/badge/{사용할 텍스트-simpleicons 코드}style=flat-square&logo={simpleicons 아이콘이름}&logoColor=white&link={링크 주소}"/></a>&nbsp
```

## 2.3 Github Stats
* **Github 통계**를 사용하여 `커밋`, `기여`, `이슈` 등 계산 결과를 **한 눈에 볼 수 있다.**

![stats](https://images.velog.io/images/daekyeong/post/fda630ad-a392-4f7d-8305-a042217037c1/image.png)

* 오늘 처음 시작해서 `Total Commits`가 2 이다. **ㅋㅋ 😁**
* 사용 방법은 아래의 코드와 같다.

```Javascript
[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username={github 아이디}&hide_title=true&show_icons=true&include_all_commits=true&disable_animations=true&theme=vue)](https://github.com/anuraghazra/github-readme-stats)
```
👉 출처 : https://github.com/anuraghazra/github-readme-stats
* 위의 사이트를 들어가 보면 **사용법과 다양한 테마**를 사용할 수 있는 방법이 친절하게 설명되어있다.

## 2.4 Solved.ac 랭크
* **백준**을 공부하는 사람들에게 **자극? 목표?**를 주는 것 같다.
* https://solved.ac/ 에서 **백준** 아이디와 연동하고 아래의 코드에 **자신의 아이디**를 넣으면 된다.

```Javascript
[![Solved.ac 프로필](http://mazassumnida.wtf/api/v2/generate_badge?boj={solved 아이디})](https://solved.ac/{solved 아이디})
```

👉 출처 : https://github.com/mazassumnida/mazassumnida

---
오늘부터 예제 실습을 시작으로 내가 하는 모든 것들을 기록해보고 싶어서 **github**을 시작했다.
아직 너무 어색하긴 하지만 꾸며야 재미도 있을 것 같았는데 너무 멋있게 꾸며져서 만족스럽다 ㅎㅎ👏
**Stats**도 점점 늘려가고 **Solved** 랭크도 얼른 높아지는 날이 다가오길 😁
## end