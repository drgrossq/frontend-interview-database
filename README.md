# Frontend Developer Interview Questions and Answers

Вопросы для подготовки к собеседованию на должность Frontend Developer. На данный момент в базе 2 вопроса.

## Содержание:

- [HTML](#html)
- [CSS](#css)

## Вопросы:

### HTML

##### 1. Для чего нужен doctype?

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

##### 1. Свойство display - основные значения и как они работают.

<details><summary><b>Ответ:</b></summary>
<p>

Свойство `display` меняет стандартный тип отображения на произвольный. `display` принимает множество значений, но основные - это: 
`none` - полностью скрывает элемент со страницы, не удаляя его при этом из HTML-разметки
`block` - размер определяется размером самого блока заданными в стилях, но сам блок занимает всю свободную ширину экрана
`inline` - элементы расположены в одну строку и их размер зависит от содержимого
`inline-block` - элементы расположены в одну строку, но элементам можно задавать размеры
`flex` - элемент становится флекс-контейнером, ведёт себя как блочный, а вложенные элементы становятся флекс-элементами
`grid` - элемент становится грид-контейнером. Снаружи грид-контейнер ведёт себя как блок. Дочерние элементы такого контейнера начинают подчиняться правилам грид-раскладки


##### Источники:

- [Спецификация](https://www.w3.org/TR/css-display-3/)
- [Дока](https://doka.guide/css/display/)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

</p>
</details>