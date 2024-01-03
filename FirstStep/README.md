# CSS 기본 문법

## 기본 선택자의 종류

|선택자|설명|예시|
|:---:|---|---|
| * |모든 태그를 선택| *{coler:red} |
|아이디|태그 속성이 아이디 속성인 값 선택| #h1{color:red} |
|클래스|태그 속성이 클래스 속성인 값 선택| .h1{color:red} |

<br>

## 색상 선택의 종류

### CSS2

|키워드|설명|
|:---:|---|
|rgb|RGB 수치 작성<br> color:rgb(20,20,20);|
|hsl|HSL수치 작성<br> color:hsl(70,70%,70%);|
|hex|RGB 16진법 코드 변환<br> color:#000000;|

<br>

### CSS3

|키워드|설명|
|:---:|---|
|rgba|RGB에 alpha(투명도) 추가<br> color:rgb(20,20,20,0.5);|
|hsla|HSL에 alpha(투명도) 추가<br> color:hsl(70,70%,70%,0.5);|

<br/>

### 색상 적용 가능한 CSS 속성명

|속성명|설명|
|:---:|---|
|color|글자색 지정 속성|
|background-color|배경색 지정 속성|
|border-color|테두리색 지정 속성|
|box-shadow|요소 그림자 지정 속성|
|text-shadow|글자 그림자 지정 속성|

<br>

## 글자 관련 속성

### color(글자색 지정 속성)

- rgb, hsl, hex 등...

### text-align(문단 가로 정렬)

|키워드|설명|
|:---:|---|
|left|글자를 왼쪽에 지정|
|right|글자를 오른쪽에 지정|
|center|글자를 가운데에 지정|
|justify|요소에 가로 폭이 있는 경우 양쪽 정렬|

### text-decoration(글자 줄 지정 속성)

|키워드|설명|
|:---:|---|
|underline|밑줄 지정|
|overline|윗줄 지정|
|line-through|가운데 줄 지정|
|none|밑줄 나오는 글자 없앰|

### text-transform(영문 대소문자 지정 속성)

|키워드|설명|
|:---:|---|
|uppercase|영문 모두 대문자 변경|
|lowercase|영문 모두 소문자 변경|
|capitalize|영문의 첫글자만 대문자로 변경|

### text-indent












