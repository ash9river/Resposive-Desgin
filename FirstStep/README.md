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

# 글자 관련 속성

## TEXT 관련 속성

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

- 수치에 따른 첫 줄 들여쓰기 혹은 내어쓰기
- default는 0

### letter-spacing

- 글자 간의 간격 조정

### word-spacing

- 단어 간의 간격 조정

### line-height

- 줄 간격 조정

### direction

- 글자 방향 전환
- **ltr**
  - 기본값(왼쪽에서 오른쪽)
- **rtl**
  - 오른쪽에서 왼쪽
 
### text-shadow

- 글자 그림자 처리
- x축 y축 번짐 색상 순이다.

```
h1{
  text-shadow:2px 2px 2px red;
}
```

## FONT 관련 속성

### font-family

- 글꼴 지정 속성

### font-size

- 글자 크기 지정 속성
- px, %, em 등

### font-weight

- 폰트가 지원해줘야 여러 굵기를 사용할 수 있다.
- 보통 100 ~ 900 사이로 100단위 사용
- **normal**
  - default
- **bold**
  - **bold**
- 숫자 지정
  - 100에서 900 사이 100단위 지정(높을수록 굵음)
 
### font-style

- **normal**
  - default
- **italic**
  - 기울게 함

### font-variant

- 소문자 => 작은 대문자
- **normal**
  - default
- **small-caps**
  - 소문자를 작은 대문자로 처리 

<br>

## 리스트 관련 속성

### list-style

- 여러 가지 있지만, url() 가능

## 배경 관련 속성

### background-color

- 배경색 지정
- color처럼 rgb, hsl, hexa 가능

### background-repeat

![111666ㅁㅁㄴ](https://github.com/ash9river/Resposive-Desgin/assets/121378532/b926c0a8-33f7-49fe-a8cd-73d94e742eca){: width=80% height=80%}

### background-position

![ㅇㅇㅁㄴㅇ](https://github.com/ash9river/Resposive-Desgin/assets/121378532/39ad0656-d2f8-4a09-952c-acf58323bf90){: width=80% height=80%}

### background-size

![asdsdad](https://github.com/ash9river/Resposive-Desgin/assets/121378532/b21514bc-8a62-49fd-af68-ceebd90b106a){: width=80% height=80%}

### background-attachment

- 스크롤해도 따라다닌다.

## 테두리 관련 속성

### border-style

|키워드|설명|
|:---:|---|
|solid|실선|
|dashed|긴 점선|
|outset|아래쪽 어둡게 처리|
|groove|파인선(3px 이상)|
|dotted|짧은 점선|
|double|두 줄 처리(2px 이상)|
|inset|위 쪽을 어둡게 처리|
|ridge|볼록한 선(3px 이상)|

### border-color

- 테두리 색 설정
- rgb, hsl, hex 등

### border

- `속기법` : width, stlye, color 한 번에 지정

```
.myContent{
  border: 1px solid black;
}
```

### border-top, border-bottom, border-left,border-right

- 한 쪽만 지정

### border-radius

- 모서리를 둥글게 한다.

## CSS2 선택자  

### 전체선택자

```css
*{
  elementName: elementValue;
}  
```

### 태그 선택자

```css
tagName{
  elementName: elementValue;
}
```

### 아이디 선택자

```css
#idName{
  elementName: elementValue;
}
```

```html
<tagName id="idName">
```

### 클래스 선택자

```css
.className{
  elementName: elementValue;
}
tagName.className{
  elementName: elementValue;
}
```

```html
<tagName class="className">
```

### 자손선택자


```css
A > B{
  elementName: elementValue;
}
```

- A의 자손인 B 선택
  
### 후손 선택자

```css
A B{
  elementName: elementValue;
}
```

- A의 후손(자손포함)인 B를 선택

### 동위선택자

```css
A + B {
  elementName: elementValue;
}
```

- A 바로 뒤에 있는 B를 선택

```css
C ~ D {
  elementName: elementValue;
}
```

- C 뒤에 있는 모든 D를 선택

### 속성선택자

```css
/* 태그의 속성명과 속성값이 같은 경우 */
tagName[elementName = elementValue]{
  elementName: elementValue;
}

/* 속성값으로 시작하는 단어 찾아 적용 */
tagName[elementName ^= elementValue]{
  elementName: elementValue;
}

/* 속성값으로 끝나는 단어 찾아 적용 */
tagName[elementName &= elementValue]{
  elementName: elementValue;
}


/* 속성값이 포함되는 단어 찾아 적용 */
tagName[elementName *= elementValue]{
  elementName: elementValue;
}
```

## CSS3 선택자

### 구조 선택자

- `:first-child` : 배열된 선택자의 첫 번째 자손 선택
- `:last-child` : 배열된 선택자의 마지막 자손 선택
- `:nth-child(n)` : 배열된 선택자의 순서를 번호로 선택
  - `nth-child(-n+index)` : 1~index까지만 선택
  - `nth-child(n+index)` : index이후부터 모두 선택
- `:nth-child(odd/even)` : 배열된 선택자가 홀수/짝수이면 선택


미디어쿼리 간단히

```css
font-size: clamp(1rem, 0.3043rem + 3.4783vw, 3rem);
```
