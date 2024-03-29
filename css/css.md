#### 1. Свойство display - основные значения и как они работают.


Свойство `display` меняет стандартный тип отображения на произвольный. `display` принимает множество значений, но основные - это: 
- `none` - полностью скрывает элемент со страницы, не удаляя его при этом из HTML-разметки
- `block` - размер определяется размером самого блока заданными в стилях, но сам блок занимает всю свободную ширину экрана
- `inline` - элементы расположены в одну строку и их размер зависит от содержимого
- `inline-block` - элементы расположены в одну строку, но элементам можно задавать размеры
- `flex` - элемент становится флекс-контейнером, ведёт себя как блочный, а вложенные элементы становятся флекс-элементами
- `grid` - элемент становится грид-контейнером. Снаружи грид-контейнер ведёт себя как блок. Дочерние элементы такого контейнера начинают подчиняться правилам грид-раскладки


##### Источники:

- [Спецификация](https://www.w3.org/TR/css-display-3/)
- [Дока](https://doka.guide/css/display/)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

---

#### 2. @keyframes - для чего нужно и как использовать?


Директива `@keyframes` используется для создания _ключевых кадров_ CSS-анимаций. После ключевого слова `@keyframes` мы должны написать имя анимации. Оно понадобится нам, чтобы связать анимацию для конкретного элемента с ключевыми кадрами. Ключевые кадры могут прописываться при помощи ключевых слов from (начальный кадр) и to (конечный кадр). Если же кадров больше двух, то можно использовать проценты. Пример:

```CSS
div {
  animation: diagonal-slide 1s infinite;
}

@keyframes diagonal-slide {

  from {
    left: 0;
    top: 0;
  }

  to {
    left: 100px;
    top: 100px;
  }

}
```

##### Источники:

- [Спецификация](https://www.w3.org/TR/css-animations-1/#keyframes)
- [Дока](https://doka.guide/css/keyframes/)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes)

---

#### 3. Что делает box-sizing: border-box?

Свойство `box-sizing` определяет как вычисляется общая ширина и высота элемента. По умолчанию размером элемента считается размер контентной области. Если кроме `width` и `height` указать ещё и `padding` с `border`, то браузер посчитает размер элемента как `width + padding * 2 + border * 2 и height + padding * 2 + border * 2`. Если задать значение `border-box` для свойства `box-sizing`, то браузер изменит принцип расчёта и `padding` с `border` уже будут включены в `width` и `height`.

##### Источники:

- [Спецификация](https://www.w3.org/TR/css-sizing-3/#box-sizing)
- [Дока](https://doka.guide/css/box-sizing/)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)

---

#### 4. Разница между margin и padding?

`margin` - задаёт размер внешнего отступа вокруг элемента. Верхний и нижний отступы не работают для элементов `<span>`, `<code>` и других строчных элементов. Выход в данной ситуации — сделать строчные элементы строчно-блочными (`inline-block`) или блочными (`block`).
`padding` - устанавливает внутренние отступы со всех сторон элемента. Область отступов это пространство между содержанием элемента и его границей. Отрицательные значения не допускаются.

![CSS Box Model](../img/CSS%20Box%20Model.png)

##### Источники:

- [Спецификация по margin](https://drafts.csswg.org/css-box/#margins)
- [Спецификация по padding](https://drafts.csswg.org/css-box/#paddings)
- [Дока по margin](https://doka.guide/css/margin/)
- [Дока по padding](https://doka.guide/css/padding/)
- [MDN по margin](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)
- [MDN по padding](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)

---

#### 5. Чем border отличается от outline?

`outline` - это линия за пределами рамки элемента и в отличии от `border` не влияет на размеры элемента т.к. `outline` не является частью блочной модели CSS. 

##### Источники:

- [Спецификация по border](https://www.w3.org/TR/css-backgrounds-3/#propdef-border)
- [Спецификация по outline](https://www.w3.org/TR/css-ui-4/#outline-props)
- [Дока по border](https://doka.guide/css/border/)
- [Дока по outline](https://doka.guide/css/outline/)
- [MDN по border](https://developer.mozilla.org/en-US/docs/Web/CSS/border)
- [MDN по outline](https://developer.mozilla.org/en-US/docs/Web/CSS/outline)