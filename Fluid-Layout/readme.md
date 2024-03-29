# 유동형 레이아웃

## 다루는 내용

- 반응형 웹 디자인에 비례형 레이아웃이 필요한 이유
- 팍샐 기반의 요소 폭을 비례 비율로 변환하기
- 픽셀 기반의 타이포그래피 크기를 em 기반으로 변환하기
- 요소에 대한 컨텍스트를 찾는 방법
- 이미지를 유동적으로 만드는 방법
- 다양한 화면 크기에 맞게 이미지를 제공하는 방법
- 미디어 쿼리로 유동형 이미지와 유동형 레이아웃을 작업하는 방법
- CSS grid 시스템을 사용해 반응형 레이아웃 작성하기

## 반응형 웹 디자인에 비례형 레이아웃이 필요한 이유

- 다양한 뷰포트 등장

## 고정 레이아웃을 비례형 레이아웃으로 수정

### 유동적 그리드를 다루는 공식 

$$
  target \div context = result
$$

```css
#wrapper {
  margin-right: auto;
  margin-left: auto;
  width: 960px;
}
```
![KakaoTalk_20240107_151342936](https://github.com/ash9river/Resposive-Desgin/assets/121378532/4dfeff24-1d68-4b0e-bdd0-6f4bf110f72e)

- 가장 바깥쪽의 div 요소에서 뷰포트의 너비를 몇퍼센트로 바꿔야 하나?

```css
#wrapper {
  margin-right: auto;
  margin-left: auto;
  width: 96% /* 가장 바깥쪽 div 요소의 크기*/
}
```

![KakaoTalk_20240107_151433891](https://github.com/ash9river/Resposive-Desgin/assets/121378532/b8c0af3a-d14e-40cc-b444-f51d32626ec8)

## 타이포그래피를 위해 px보다는 em을 사용

```css
font-size: 100%;
font-size: 16px;
font-size: 1em;
```

- 다 같은 크기이다.


## 유동형 이미지

- 이미지의 너비와 높이를 명시적으로 기술하지 말고, 뷰포트에 맞게 이미지의 크기를 조절한다.

```css
img {
  width: 42%;
  max-width: 202px;
}
```

- wrapper에 max-width 속성을 추가하여, 디자인의 무분별한 확대를 막는다.

```css
#wrapper {
  margin-right: auto;
  margin-left: auto;
  width: 96% /* 가장 바깥쪽 div 요소의 크기*/
  max-width: 1414px;
}
```

### 유동형 그리드와 미디어 쿼리를 함께 사용

```css
@media screen and (min-width: 1001px) and (max-width: 1080px) {
#navigation ul li { font-size: 1.4em; }
}
@media screen and (min-width: 805x) and (max-width: 1000px) {
#navigation ul li { font-size: 1.25em; }
}
@media screen and (min-width: 769px) and (max-width: 804px) {
#navigation ul li { font-size: 1.1em; }
}
```

- 뷰포트의 크기에 따라 폰트 크기를 변경, 769px부터 무한대까지 네비게이션 링크를 한 줄에 표시
- 미디어 쿼리의 최신 문법이 더 직관적이다.

```css
@media (width <= 768px) {
}

@media (769px <= width <= 1000px) {
}
```

- 컨테이너 쿼리를 이용해서 뷰포트가 아니라, 특정 요소의 크기에 따라 반응적인 동작을 지정하는 방법도 있다.


