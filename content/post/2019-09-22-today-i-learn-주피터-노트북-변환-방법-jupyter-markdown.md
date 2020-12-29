---
title: Today I Learn / 주피터 노트북 변환 방법(jupyter -> markdown)
author: 류성균
date: '2019-09-22'
slug: today-i-learn-주피터-노트북-변환-방법-jupyter-markdown
categories:
  - Today I learn
tags:
  - jupyter notebook
keywords:
  - tech
---

<!--more-->


- 출처 : https://www.timlrx.com/2018/03/25/uploading-jupyter-notebook-files-to-blogdown/

blogdown으로 블로그를 운영하는데 아쉬운 건 테마, 폰트 등 수도 없지만 더 아쉬운건 파이썬을 쓰기 번거롭다는 것이다. 'reticulate' 패키지를 써도 되긴하는데 주피터 노트북도 사용 가능하다고 한다!!

1. 주피터 노트북 변환

우선 변환할 주피터 노트북을 찾는다. 나 같은 경우는 테스트할 파일을 찾다가 '파이썬 라이브러리를 활용한 머신러닝' 연습했던 걸 활용해보고자 한다.

![](https://raw.githubusercontent.com/rhyeu/blog/master/content/img/covert_md.PNG)

주피터 노트북을 작성한 뒤 아나콘다 프롬프트를 켠다. 변환할 주피터 노트북이 있는 장소로 이동한 뒤 아래의 코드를 실행한다.

```
jupyter nbconvert --to markdown "변환할 파일 이름(확장자까지)"
```

그럼 md파일이 생성되는 것을 확인할 수 있다.

그 다음은 보통 포스팅을 올리듯 'new post'를 올릴 준비를 하고 아래에 변환된 md 파일 내용을 붙여넣으면 된다!!1

아래의 링크는 실제 생성된 포스팅이다.
https://rhyeu.netlify.com/2019/09/22/today-i-learn-example/

