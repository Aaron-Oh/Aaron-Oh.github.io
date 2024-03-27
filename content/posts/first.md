---
title: "Hugo로 첫 포스트 작성하기"
date: 2024-03-12T09:00:00
lastmod: "2024-03-12"
draft: false
categories: ["블로그 시작하기"]
tags: ["Hugo", "첫 포스트", "블로그"]
series: ["Hugo 블로그 구축"]
image: "/images/default.jpg"
hideFromHomePage: false
---

Hugo를 사용하여 나의 첫 번째 블로그 포스트를 작성하는 방법을 소개합니다.

Hugo는 간단하고 빠른 정적 사이트 생성기로, 마크다운을 사용하여 콘텐츠를 작성할 수 있습니다. Hugo와 GitHub Pages를 함께 사용하면, 복잡한 서버 설정 없이도 개인 블로그를 운영할 수 있습니다.

<!--body-->

## 시작하기

Hugo를 설치하고 새로운 사이트를 생성하는 것부터 시작해보겠습니다. 다음 단계를 따라해 보세요:

1. Hugo 설치: [Hugo 공식 문서](https://gohugo.io/getting-started/installing/)를 참조하여 시스템에 Hugo를 설치합니다.
2. 새 사이트 생성: 터미널에서 다음 명령어를 실행하여 새 사이트를 생성합니다.

```bash
hugo new site myblog
