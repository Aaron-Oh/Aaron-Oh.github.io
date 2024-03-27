---
title: "확장된 마크다운 문법 사용하기"
date: 2024-02-12T09:00:00
lastmod: "2024-02-12"
draft: false
categories: ["블로그 시작하기"]
tags: ["Hugo", "마크다운", "markdown"]
series: ["Hugo 블로그 구축"]
image: "/images/default.jpg"
hideFromHomePage: false
---

<!--body-->
# Code
## Code in line
Example: basic: "`name`"
options: you can add options featuring as what you want to highlight
just add (primary), (tip), (warning), (success), (danger) **with one white space**

`name (primary)`  

`name (tip)`  

`name (warning)`  

`name (success)`  

`name (danger)`  


## Example of code block
```python
close #클릭하면 열립니다
import sys
input = sys.stdin.readline

def getUserInput():
    n = input()
    print(f'user input is : {n}')

if __name__ == '__main__':
    getUserInput()
```

If you add 'close' option into the first line of the code block, you can roll up the code block


### 3개부터는 애니메이션 효과가 사라집니다.
#### 대신 볼드체로 강조됩니다.
##### 또한 개수가 증가할 수록 글자의 크기가 작아집니다.
As you can see, more than 2 #, it just be bolder and smaller 

🥳 이모지 테스트
😤 이모지 테스트

## with & without count
1. 아니요??
2. 네 맞습니다
   
- 저는 바보는 아닙니다
- 바보
- 맞을 수도
  
---
# quotation

> 이것은 인용 예시입니다.
>   기본 인용은 회색으로 표시됩니다.
>   마찬가지로 옵셥을 추가할 수 있습니다.


> primary
>  'primary' 예약어를 사용한 경우입니다.
>   주요 문단입니다

> tip
>  'tip' 예약어를 사용한 경우입니다.
>   팁 문단입니다

> warning
>  'warning' 예약어를 사용한 경우입니다.
>   경고 문단입니다

> success
>   'success' 예약어를 사용한 경우입니다.
>   성공 문단입니다

> danger
>   'danger' 예약어를 사용한 경우입니다.
>    실패(위험) 문단입니다

---
# Picture
Basically, picture has a shadow. so if you don't want to add it, just add `_no` at the end of the text in quotation

1. title with shadow
   ```markdown
   ![photo](/images/example.jpeg 'title')
    ```

    result:
    ![photo](/images/example.jpeg 'title')

2. title without shadow
   ```markdowm
   ![photo](/images/example.jpeg 'title_no')
    ```

    result:
    ![photo](/images/example.jpeg 'title_no')

3. without title but shadow
   ```markdown
   ![photo](/images/example.jpeg)
    ```

    result:
    ![photo](/images/example.jpeg)

4. without title and shadow
   ```markdown
   ![photo](/images/example.jpeg '_no')
    ```

    result:
    ![photo](/images/example.jpeg '_no')


---
# Tap
## example of tap
1. basic use
    ```markdown
    ::: tabs
    @tab jay
    Hi I'm jay!
    @tab lay
    I'm lay!
    @tab kelvin
    yeah I'm kelvin!
    :::
    ```

    result:

    ::: tabs
    @tab jay
    Hi I'm jay!
    @tab lay
    I'm lay!
    @tab kelvin
    yeah I'm kelvin!
    :::

2. option `:active`
   
   ```markdown
    ::: tabs
    @tab jay
    Hi I'm jay!
    @tab:active lay
    I'm lay!
    @tab kelvin
    yeah I'm kelvin!
    :::
    ```

    result:

    ::: tabs
    @tab jay
    Hi I'm jay!
    @tab:active lay
    I'm lay!
    @tab kelvin
    yeah I'm kelvin!
    :::

3. option `#id`
   
    you can add 'id' into the tap container and if two containers have same 'id', they share tap switching event.

    ```markdown
    ::: tabs#install

    @tab npm

    npm을 사용하여 xxx설치

    @tab Homebrew

    Homebrew를 사용하여 xxx설치

    @tab MacPorts

    MacPorts를 사용하여 xxx설치

    :::
    ```

    ```markdown
    ::: tabs#install

    @tab npm

    npm을 사용하여 yyy설치

    @tab Homebrew

    Homebrew를 사용하여 yyy설치

    @tab MacPorts

    MacPorts를 사용하여 yyy설치

    :::
    ```

    result: 

    ::: tabs#install

    @tab npm

    npm을 사용하여 xxx설치

    @tab Homebrew

    Homebrew를 사용하여 xxx설치

    @tab MacPorts

    MacPorts를 사용하여 xxx설치

    :::

    ::: tabs#install

    @tab npm

    npm을 사용하여 yyy설치

    @tab Homebrew

    Homebrew를 사용하여 yyy설치

    @tab MacPorts

    MacPorts를 사용하여 yyy설치

    :::


---
# mermaid
you can draw graph and flow chart with mermaid.

    ```mermaid: true
    flowchart LR
        A -- text --> B -- text2 --> C
    ```

result:

mermaid: true
    flowchart LR
        A -- text --> B -- text2 --> C

more usage in here: https://mermaid.js.org/#/

---
# math
use mathjax: https://www.mathjax.org

1. math in line
   
    ```math: true
    "<!-- '\(' 와 '\)' 로 인라인 수식의 시작과 끝을 표시 -->"
    행내 공식입니다：\( x = {-b \pm \sqrt{b^2-4ac} \over 2a} \)
    ```

2. math in block
   
    ```math: true
    "<!-- '$$' 와 '$$' 로 수식 블록의 시작과 끝을 표시 -->"
    블럭 내 공식입니다：$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$
    ```


