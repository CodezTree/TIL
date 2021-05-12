# Markdown 문법 정리

## Markdown 장점

1. 쉬운 문법
2. 문서 관리 쉬움
3. 다양한 프로그램과 플랫폼에서 지원

---

## Markdown Syntax

### ▶︎ Header (제목)

<code>h1</code>에서 <code>h6</code>까지 제목을 표현할 수 있다.

```
# 헤더 1
## 헤더 2
...

###### 헤더 6
```

결과

____

# 헤더 1

## 헤더 2

###### 헤더 6

---

문단 제목은 주제목은 `===` 소제목은 `---`를 이용합니다.

```
주제목
===
소제목
---
```

주제목
===
소제목
---

---
<br/>

### ▶︎ Line Break (줄바꿈)

기본적인 마크업 언어에서는 띄어쓰기를 2번 하거나, `<br>`를 이용하면 줄바꿈을 할 수 있습니다. 주석이 있다면 주석 뒤에 두 번을 입력해야 제대로 인식이 됩니다.

```
안녕하세요. 제 이름은 CodezTree입니다. <!--띄어쓰기 2번-->  
만나서 반갑습니다. 잘 지내시나요.  
보고싶네요 WhiteKiwi씨.<br>
TIL는 재밌을 지도 모르겠어요.
```

안녕하세요. 제 이름은 CodezTree입니다.  <!--띄어쓰기 2번-->  
만나서 반갑습니다. 잘 지내시나요.  
보고싶네요 WhiteKiwi씨.<br>
TIL는 재밌을 지도 모르겠어요.

<br>

### ▶︎ Horizontal Line (구분선)

<code>---</code> 혹은 <code>\***</code>를 이용하면 됩니다.<br/>

---
구분
***
구분
***

<br/>

### ▶︎ Emphasis (강조)

순서대로

\**( \_ \_ ), ****( \_\_ __ ), ~~~~, <code><u></u></code>

<code>\<em></code> - 이텔릭체, <code>\<strong></code> - 두껍게,<code>\<del></code> - 취소선, <code>\<u></u></code> - 밑줄로 대응됩니다.

```
이텔릭체는 *Asterisks(별표)* 혹은 _UnderBar(언더바)_를 사용할 수 있습니다.
두껍게는 **별표 두개** 혹은 __언더바 두개__를 사용하세요.
두가지를 **_한꺼번에!_는 이렇게** 사용하세요.
반대로 *__이렇게__도 가능하지요*.
취소선은 ~~Tilde(물결표시)~~를 사용하세요!
<u>밑줄</u>는 요로콤 =)
```

>이텔릭체는 *Asterisks(별표)* 혹은 _Underscore(언더바)_ 를 사용할 수 있습니다.<br/>
두껍게는 **별표 두개** 혹은 __언더바 두개__ 를 사용하세요.<br/>
두가지를 **_한꺼번에!_ 는 이렇게** 사용하세요.<br/>
반대로 *__이렇게__ 도 가능하지요*<br/>
취소선은 ~~Tilde(물결표시)~~를 사용하세요!<br/>
<u>밑줄</u>는 요로콤 =)<br/>

<br/>

### ▶︎ List (목록)

<code>1. 2. ..</code>는 순서 목록에 대응 <br/>
<code>-, *, +</code>는 순서 필요 없는 목록에 대응

```
1. 순서가 필요한 목록
2. 순서가 필요함
  - 순서 필요 없음. sub_1
  - 순서 필요 없음. sub_2
3. 순서가 필요함
  1. 순서가 필요함. sub_1
  2. 순서가 필요함. sub_2

- 순서 필요 없음
  - Hyphen(대쉬)
  * Asterisks(별표)
  + Plus Sign(더하기)
```

1. 순서가 필요한 목록
2. 순서가 필요함
  - 순서 필요 없음. sub_1
  - 순서 필요 없음. sub_2
3. 순서가 필요함
  1. 순서가 필요함. sub_1
  2. 순서가 필요함. sub_2

- 순서 필요 없음
  - Hyphen(대쉬)
  * Asterisks(별표)
  + Plus Sign(더하기)

<br/>

### ▶︎ Link (링크)

일반적으로 <code>\[텍스트](링크)</code> 로 사용합니다.<br/>
링크만 바로 연결하고 싶다면 <code><></code>를 사용하세요.<br/>
<code>[]</code>를 이용해 [참조링크]를 사용합니다.


```
[Google](https://google.com)

[Github](https://github.com)

[md 파일에 상대적 위치](../OOP/SOLID.md)

이렇게 문서에서 [참조 링크]를 넣을 수 있습니다.
꺽쇠는 <https://naver.com> 자동링크를 삽입합니다.

[참조 링크]: https://google.com "구글로 링킹됩니다."
```

[Google](https://google.com)

[Github](https://github.com)

[md 파일에 상대적 위치](../OOP/SOLID.md)

이렇게 문서에서 [참조 링크]를 넣을 수 있습니다.<br/>
꺽쇠는 <https://naver.com> 자동링크를 삽입합니다.<br/>

[참조 링크]: https://google.com "구글로 링킹됩니다."

<br/>

### ▶︎ Image (이미지)

이미지는 링크와 비슷합니다. 하지만 <code>!</code>가 앞에 붙습니다.

```
![대체 텍스트](https://t1.daumcdn.net/thumb/R1280x0/?fname=http://t1.daumcdn.net/brunch/service/user/5xq2/image/0lp8RLaJ2IgctTWVl2nEa-JRCSc.jpg "링크 설명 입니다!")

![Squirrel][cute]

[cute]: https://postfiles.pstatic.net/MjAxODA1MDZfNjcg/MDAxNTI1NTUxNzQ5ODQ3.T9KWivdyNoofKnyIJxv1JYrJeBRuKJ-eFnWllhhMkXEg.gG415bxMbmCICHivI91a6MNs0wI8GOWiMaPW0hkyXUUg.JPEG.jadekim925/Streifenhoernchen.jpg?type=w966 "Cute Squirrel"
```

![대체 텍스트](https://t1.daumcdn.net/thumb/R1280x0/?fname=http://t1.daumcdn.net/brunch/service/user/5xq2/image/0lp8RLaJ2IgctTWVl2nEa-JRCSc.jpg "링크 설명 입니다!")

![Squirrel][cute]

[cute]: https://postfiles.pstatic.net/MjAxODA1MDZfNjcg/MDAxNTI1NTUxNzQ5ODQ3.T9KWivdyNoofKnyIJxv1JYrJeBRuKJ-eFnWllhhMkXEg.gG415bxMbmCICHivI91a6MNs0wI8GOWiMaPW0hkyXUUg.JPEG.jadekim925/Streifenhoernchen.jpg?type=w966 "Cute Squirrel"

이미지에 링크를 넣으려면 <code>\[!\[텍스트](이미지링크)](이동링크)</code>를 사용합니다.

```
[![귀여운사람](./images/cuteman.jpg)](https://google.com)
```
[![귀여운사람](./images/cuteman.jpg)](https://google.com)

<br/>

### ▶︎ 코드 하이라이트

#### Inline(인라인) 코드 강조

숫자 1번 키 옆 물결 버튼 아래 <code>\`</code>  기호를 이용합니다.<br/>
맥은 한글 일때 `₩` 기호가 표시됩니다. 영문으로 바꾸어주면 쓸 수 있습니다!

```
나는 `사람`이고 넌`신`이야.
```

나는 `사람`이고 넌`신`이야.

#### Block(블럭) 코드 강조

<code>\`\`\`</code> 를 감싸줍니다. 처음 기호 오른쪽에 코드 종류도 적어줍니다.
```
```html
<a href="https://www.google.co.kr/" target="_blank">Google</a>
```.
```

```html
<a href="https://www.google.co.kr/" target="_blank">Google</a>
```

<br/>

### ▶︎ Table (표)

`|` 로 칸을 나눕니다.<br/>
헤더를 구분할 때 `---` 기호가 필요합니다.<br/>
헤더 칸을 나누면서 `:` 기호로 셀(열)에 있는 내용을 정렬합니다 - `---` 왼쪽에 넣으면 좌측 정렬, 오른쪽은 우측정렬, 양측은 중앙정렬을 수행합니다.<br/>
가장 우측의 `|` 는 생략 가능합니다. <br/>

```
|name|value|quantity|
|---|:---:|---:|
|'Chulsoo'|10|2|
|'Apple'|100|10|
|'Trash'||100|
```

|name|value|quantity|
|---|:---|:---:|
|'Chulsoo'|10|2|
|'Apple'|100|10|
|'Trash'||100|

<br/>

### ▶︎ BlockQuote (인용문)

`>`를 사용합니다.

```
> 누군가가 말했어
>> 삶에 대해서 말이야
>>> 그냥 생각없이 사는게 최고라고.
>>> 흘러가는 대로 사는거라고.
>>> 순간 순간을 즐기라고.
```

> 누군가가 말했어
>> 삶에 대해서 말이야
>>> 그냥 생각없이 사는게 최고라고.  
>>> 흘러가는 대로 사는거라고.  
>>> 순간 순간을 즐기라고.

<br/>

### ▶︎ 원시 HTML 문법

마크다운 문법이 아닌 HTML 문법을 사용 가능합니다.

```
<details>
<summary>Click to expand</summary>

<ul>
    <li>WhatEver</li>
    <li>HowEver</li>
</ul>

</details>
```

<details>
<summary>Click to expand</summary>

<ul>
    <li>WhatEver</li>
    <li>HowEver</li>
</ul>

</details>

<br/>

### ▶︎ Markdown에 귀여운 이모지!

이모지를 간단한 코드로 삽입할 수 있습니다. `:이모지tag:`  
이모지 리스트는 [여기](https://gist.github.com/rxaviers/7360908)에서 확인할 수 있습니다. (특정 Application에서 사용 불가능한 이모지도 있습니다.)

```
나는 행복해!! :joy:

캠핑을 가고 싶은데...? :tent:
```

나는 행복해!! :joy:

캠핑을 가고 싶은데...? :tent:
