---
layout: post
title: "Mac M1 이슈 정리"
author: "Hyewon"
categories: project
tags: [FE, NodeJS]
---

맥북 M1으로 개발환경을 구축하면서 겪은 이슈 정리하는 포스팅

<br>

### 1. NodeJS 버전 이슈

M1에서 기존 프로젝트를 clone해서 npm install하는 과정에서 node version 이슈가 있었다.<br>
구글링을 통해 알아낸 결과 M1에서는 15이상의 버전을 지원하고, node 15미만의 버전으로 설치할 경우, Rosetta2를 이용하여 설치해야한다.

즉, 해결방법은 두가지가 있다.

1. 15이상의 node 버전으로 설치
2. node 버전 15미만일 경우 Rosetta2를 사용해 설치한다.

Rosetta2 사용법 : 터미널 옵션 -> 정보가져오기 -> `Rosetta를 사용하여 열기`

<!-- ---
layout: post
title: "나의 첫 회사, 첫 프로젝트 만또(Mantto)"
author: "Hyewon"
categories: project
tags: [FE, ReactNative, Application]
image: mantto.jpg
---

만또 프로젝트(React Native 기반)의 프론트엔드 개발을 진행하면서 공부한 내용 혹은 겪은 일들을 정리하려 한다.<br>
[Github 소스코드](https://github.com/yirangsProject/frontend)

### FE 개발 환경

프론트엔드 개발은 ios, android를 한번에 개발 할 수 있는 `react-native` `프레임워크`를 사용한다. 백앤드를 GraphQL로 설계해 `백앤드와의 통신`을 `Apollo Graphql`로 한다. Apollo에 있는 `cache`로 `주된 전역 변수 관리`를 하고 간단하고 `일시적인 전역변수 관리`의 경우 `Redux`를 사용한다.

- Apollo Client

백앤드 통신

- Apollo Graphql

디버깅 툴

- Reactroton

### 기술을 제대로 학습하기에 Docs만한게 없다. -->
