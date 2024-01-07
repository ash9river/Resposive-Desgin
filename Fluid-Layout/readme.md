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







    




