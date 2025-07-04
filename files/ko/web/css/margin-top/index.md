---
title: margin-top
slug: Web/CSS/margin-top
---

{{CSSRef}}

**`margin-top`** [CSS](/ko/docs/Web/CSS) 속성은 요소의 위쪽에 [바깥 여백 영역](/ko/docs/Web/CSS/CSS_box_model/Introduction_to_the_CSS_box_model)margin area을 설정합니다. 양수 값은 인접 요소와 거리를 넓히고, 음수 값은 더 좁힙니다.

{{InteractiveExample("CSS Demo: margin-top")}}

```css interactive-example-choice
margin-top: 1em;
```

```css interactive-example-choice
margin-top: 10%;
```

```css interactive-example-choice
margin-top: 10px;
```

```css interactive-example-choice
margin-top: 0;
```

```html interactive-example
<section id="default-example">
  <div id="container">
    <div class="row"></div>
    <div class="row transition-all" id="example-element"></div>
    <div class="row"></div>
  </div>
</section>
```

```css interactive-example
#container {
  width: 300px;
  height: 200px;
  display: flex;
  align-content: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}

.row {
  height: 33.33%;
  display: inline-block;
  border: solid #ce7777 10px;
  background-color: #2b3a55;
  flex-shrink: 0;
}

#example-element {
  border: solid 10px #ffbf00;
  background-color: #2b3a55;
}
```

{{HTMLElement("span")}}, {{HTMLElement("code")}} 등 [비대체](/ko/docs/Web/CSS/CSS_images/Replaced_element_properties)non-replaced 인라인 요소에는 효과가 없습니다.

## 구문

```css
/* <length> 값 */
margin-top: 10px; /* 절대 길이 */
margin-top: 1em; /* 글씨 크기에 상대적 */
margin-top: 5%; /* 가장 가까운 블록 컨테이너의 너비에 상대적 */

/* 키워드 값 */
margin-top: auto;

/* 전역 값 */
margin-top: inherit;
margin-top: initial;
margin-top: unset;
```

`margin-top` 속성은 키워드 `auto`, `<length>`, `<percentage>`를 사용해 설정할 수 있습니다. 값은 양수, 0, 음수가 가능합니다.

### 값

- {{cssxref("&lt;length&gt;")}}
  - : 바깥 여백 크기의 고정 값.
- {{cssxref("&lt;percentage&gt;")}}
  - : 바깥 여백 크기와 블록 컨테이너 너비의 비율.
- `auto`
  - : 브라우저가 적절한 값 선택. {{cssxref("margin")}}을 참고하세요.

### 형식 구문

{{csssyntax}}

## 예제

```css
.content {
  margin-top: 5%;
}
.sidebox {
  margin-top: 10px;
}
.logo {
  margin-top: -5px;
}
#footer {
  margin-top: 1em;
}
```

## 명세

{{Specifications}}

{{cssinfo}}

## 브라우저 호환성

{{Compat}}
