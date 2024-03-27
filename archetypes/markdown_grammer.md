클라우드 만세 
인공지능 시스템 만만세 

"잠실코딩개발협동조합 창단 멤버" 탠저린 프린스입니다.
제발 신이시여 제발 이제 좀 되게해주세요.
저 일주일 고생했어요.
개행은 왜 안 되는거야
<!--more-->
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
> 기본 인용은 회색으로 표시됩니다.
> 마찬가지로 옵셥을 추가할 수 있습니다.


> primary
> 'primary' 예약어를 사용한 경우입니다.
> 주요 문단입니다

> tip
> 'tip' 예약어를 사용한 경우입니다.
> 팁 문단입니다

> warning
> 'warning' 예약어를 사용한 경우입니다.
> 경고 문단입니다

> success
> 'success' 예약어를 사용한 경우입니다.
> 성공 문단입니디ㅏ

> danger
> 'danger' 예약어를 사용한 경우입니다.
> 실패(위험) 문단입니디ㅏ

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

    ```maekdown
    ::: tabs#install

    @tab npm

    npm을 사용하여 xxx설치

    @tab Homebrew

    Homebrew를 사용하여 xxx설치

    @tab MacPorts

    MacPorts를 사용하여 xxx설치

    :::
    ```

    ```maekdown
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
    ```mermaid
    flowchart LR
        A -- text --> B -- text2 --> C
    ```

result:
    flowchart LR
        A -- text --> B -- text2 --> C

more usage in here: https://mermaid.js.org/#/

---
# math
use mathjax: https://www.mathjax.org
1. math in line
    ```math
    <!-- 用 '\(' 和 '\)' 表示行内公式的起始和结束 -->
    这是一个行内公式：\( x = {-b \pm \sqrt{b^2-4ac} \over 2a} \)
    ```

2. math in block
    ```math
    <!-- 用 '$$' 和 '$$' 表示公式块的起始和结束 -->
    这是一个公式块：$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$
    ```


