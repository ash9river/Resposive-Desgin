# 미디어 쿼리

## 미디어 쿼리로 판단할 수 있는 사항

- `width` : 뷰포트 너비
- `height` : 뷰포트 높이
- `device-width` : 렌더링되는 표면(디바이스 스크린)의 너비
- `device-height` : 렌더링되는 표면(디바이스 스크린)의 높이
- `orientation` : 디바이스의 세로/가로 방향 여부
- `aspect-ratio` : 높이에 대한 너비의 비율로, 뷰포트에 기반한다. 16:9의 와이드 스크린이면 `aspect-ratio:16/9`로 표시된다.
- `device-aspect-ratio` : `aspect-ratio`와 유사하나, 렌더링되는 표면(디바이스 스크린) 기반.
- `color` : 색상 구성요소당 비트의 수. `min-color:16`은 디바이스의 16비트 색상 지원 여부를 판단한다.
- `color-index` : 디바이스의 색상 조회 테이블에 있는 항목의 수. 값은 음이 아닌 정수.
- `monochrome` : 모노크롬 프레임 버퍼의 픽셀당 비트수. 값은 음이 아닌 정수.
- `resolution` : 스크린이나 프린터의 해상도를 테스트. cm당 도트 수도 가능하다.
- `scan` : TV에 특정적인 기능으로, progressive or interlace.
- `grid` : 디바이스가 grid 기반인지 or 비트맵 기반인지를 나타낸다.

- scan과 grid를 제외한 위의 모든 기능은 범위를 제한하기 위해 min이나 max 접두사를 사용할 수 있다.
- CSS의 @import 기능을 사용하면 http 요청이 증가하기 때문에 로딩속도에 영향을 미쳐 느려진다.
- 기존 스타일 시트에 간단한 미디어 쿼리 스타일을 추가하여,, 반응형 디자인을 만든다.

```css
@media screen and (max-width: 760px) { STYLE}
```
