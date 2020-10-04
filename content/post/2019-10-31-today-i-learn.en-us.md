---
title: Today_I_Learn
author: 류성균
date: '2019-10-31'
slug: today-i-learn.en-us
categories:
  - Today I learn
  - R
tags:
  - R
  - Launguage
keywords:
  - tech
---

- 출처 : https://www.lucypark.kr/blog/2012/05/31/r-console-language-configuration/
R을 지웠다 깔 때마다 매번 찾아봐서 정리하려고 한다. R을 깔면 자동으로 한국어가 출력되도록 세팅되어있는데 가끔 출력 언어가 깨져서 어떤 오류가 났는 지 확인이 어려운 경우가 있어 매번 귀찮게 바꿔줘야 한다..

바꾸는 방법은 간단하다.

’관리자 권한으로 실행’된 텍스트 에디터에서 ‘C:/Program Files/R/R-3.6.1/etc/Rconsole’ 파일을 연다.

중간 부분에 있는 메시지 언어 설정 내용을 아래와 같이 바꿔준다.

## Language for messages
language = en
R을 재실행한다.