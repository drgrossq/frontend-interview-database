# Frontend Developer Interview Questions and Answers

Вопросы для подготовки к собеседованию на должность Frontend Developer. На данный момент в репозитории 3 вопроса.

## Содержание:

- [HTML](#html)
- [CSS](#css)

## Вопросы:

### HTML

#### 1. Для чего нужен doctype?

<details><summary><b>Ответ:</b></summary>
<p>

Согласно спецификациям HTML и XHTML тег DOCTYPE сообщает валидатору, какую именно версию (X)HTML вы используете в своей странице. Этот тег должен всегда находиться в первой строке каждой страницы. Что бы сообщить браузеру, что мы используем тип документа HTML 5, надо указывать `<!DOCTYPE html>`

##### Источники:

- [Спецификация](https://html.spec.whatwg.org/multipage/syntax.html#the-doctype)
- [Дока](https://doka.guide/html/doctype/)
- [MDN](https://developer.mozilla.org/en-US/docs/Glossary/Doctype)

</p>
</details>

### CSS

#### 1. Свойство display - основные значения и как они работают.

<details><summary><b>Ответ:</b></summary>
<p>

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

</p>
</details>

#### 2. @keyframes - для чего нужно и как использовать?

<details><summary><b>Ответ:</b></summary>
<p>

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

</p>
</details>

#### 3. Что делает box-sizing: border-box?

<details><summary><b>Ответ:</b></summary>
<p>

Свойство `box-sizing` определяет как вычисляется общая ширина и высота элемента. По умолчанию размером элемента считается размер контентной области. Если кроме `width` и `height` указать ещё и `padding` с `border`, то браузер посчитает размер элемента как `width + padding * 2 + border * 2 и height + padding * 2 + border * 2`. Если задать значение `border-box` для свойства `box-sizing`, то браузер изменит принцип расчёта и `padding` с `border` уже будут включены в `width` и `height`.

##### Источники:

- [Спецификация](https://www.w3.org/TR/css-sizing-3/#box-sizing)
- [Дока](https://doka.guide/css/box-sizing/)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)

</p>
</details>