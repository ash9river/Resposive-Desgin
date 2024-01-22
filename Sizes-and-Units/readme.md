# Sizes and Units

## Units

|Name|Abbre|
|:---:|:---:|
|pixels|px|
|percentages|%|
|root em|rem|
|em|em|
|viewport height|vh|
|viewport width|vw|

## 크기 계산과 단위

### px

- `절대 길이` : 유저 세팅을 무시한다.

## px을 사용하면 안되는 이유

- 반응형 웹사이트에서 px을 사용하면, 고정된 크기로는 제대로 반응형을 나타낼 수 없다.
- 
### Viewport Lengths

- 뷰포트의 길이에 맞게 길이를 조절한다.
- **vh, vw, vmin, vmax**...

### Font-Relative Lengths

- 폰트 상대적 길이
- **rem, em**

### %

- 특수 사례로, 부모 컨테이너에 대한 %이다.
- 유닛에 가장 먼저 적용된다.
- 해당 요소의 position에 따라서 결정된다.
- 만약 `position:fiexed`이면 컨테이닝 블록은 `viewport`로 인식된다.

> 💡 position:fixed가 적용된 요소에 %를 사용하면 컨테이닝 블록은 뷰포트라는 것을 확인할 수 있다.












