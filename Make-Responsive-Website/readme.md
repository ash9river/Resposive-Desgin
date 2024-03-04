# Make Responsive Website

## Hardware pixel vs Software pixel

![image](https://github.com/ash9river/Resposive-Desgin/assets/121378532/9734b8ab-c98b-4471-bf2e-c414f8edf51e)


- 크롬의 개발자 도구를 켜서 보면 너비를 375px이라 정의되어 있지만, **CSS**에서는 980px이라 나와 있다.
- 브라우저는 기본적으로 갖는 하드웨어 픽셀을 식별하고, 해당 픽셀 값을 1인치가 96px이라는 절대길이의 논리식을 기반으로 하여 변환한다.
- 이는 모니터나 데스크톱 기기에서는 완벽하게 작동하지만, 모바일 폰의 경우에는 웹사이트가 이런 식으로 너무 작게 표시되는 결과가 발생한다.
- 현대 모바일 폰의 픽셀 밀도가 매우 높기 때문에, 높은 픽셀 밀도, 즉 좁은 공간에 들어가는 픽셀의 양이 많으면 문제가 발생하게 된다.
  - 픽셀을 인치로 변환하여 기기에 표시할 정보의 양을 지정하는 방법이 더 이상 정상적으로 작동하지 않게 된다.
 
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- 메타태그에 뷰포트 추가로 해결

### viewport

- 뷰포트 메타 태그는 기기 뷰포트에 맞게 웹사이트를 조정한다.
- 그러나 뷰포트 메타 태그는 디자인을 변경할 수 없고, 픽셀 비율에 따른 픽셀 변환만으로 웹의 디스플레이 방식을 조정할 수만 있다.

### media query

- 너비에 맞게 특정 규칙을 지정할 수 있다.














