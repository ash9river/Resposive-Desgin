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

![image](https://github.com/ash9river/Resposive-Desgin/assets/121378532/a42e1402-2d56-418c-9b17-61c7da91f316)


> 💡 position:fixed가 적용된 요소에 %를 사용하면 컨테이닝 블록은 뷰포트라는 것을 확인할 수 있다.

- 만약 `position:absolute`이면 컨테이닝 블록으로서 조상(Ancestor)의 컨텐츠와 안쪽 여백의 너비(padding)를 기준으로 삼는다.
- `position:absolute`인 요소의 컨테이닝 블록은 position이 가장 인접한 조상이 된다.

![image](https://github.com/ash9river/Resposive-Desgin/assets/121378532/de2ada0b-bcd2-42f0-be51-4c223d7413a2)

- 만약 `position:static` 또는 `position:relative`이면 조상의 컨텐츠를 기준으로 삼는다.
- 조상은 block level element가 된다.

![image](https://github.com/ash9river/Resposive-Desgin/assets/121378532/d851a4eb-da43-436b-ac5e-0b6186c90b08)








