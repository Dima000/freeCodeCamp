---
id: bad87fee1348bd9aedf08746
title: Inherit Styles from the Body Element
challengeType: 0
videoUrl: https://scrimba.com/c/c9bmdtR
forumTopicId: 18204
localeTitle: Наследовать стили из элемента тела
---

## Description
<section id='description'>
Теперь мы доказали, что каждая HTML-страница имеет элемент <code>body</code> , а ее элемент <code>body</code> также может быть связан с CSS. Помните, вы можете стилизовать свой элемент <code>body</code> же, как любой другой элемент HTML, и все ваши другие элементы наследуют стили вашего <code>body</code> .
</section>

## Instructions
<section id='instructions'>
Во-первых, создайте элемент <code>h1</code> с текстом <code>Hello World</code> Затем дадим все элементы на вашей странице цвета <code>green</code> , добавив <code>color: green;</code> к объявлению стиля вашего <code>body</code> . Наконец, придайте вашему <code>body</code> элемент семейства шрифтов <code>monospace</code> , добавив <code>font-family: monospace;</code> к объявлению стиля вашего <code>body</code> .
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Creaza un element <code>h1</code>.
    testString: assert(($("h1").length > 0));
  - text: Elemetul tau <code>h1</code> trebuie sa contina textul <code>Hello World</code>.
    testString: assert(($("h1").length > 0 && $("h1").text().match(/hello world/i)));
  - text: Asigurate ca elemetul <code>h1</code> are un tag de inchidere.
    testString: assert(code.match(/<\/h1>/g) && code.match(/<h1/g) && code.match(/<\/h1>/g).length === code.match(/<h1/g).length);
  - text: Atribuie elementului <code>body</code> proprietatea de stil <code>color</code> cu valoarea <code>green</code>.
    testString: assert(($("body").css("color") === "rgb(0, 128, 0)"));
  - text: Atribuie elementului <code>body</code> proprietatea de stil <code>font-family</code> cu valoarea <code>monospace</code>.
    testString: assert(($("body").css("font-family").match(/monospace/i)));
  - text: Elentul tau <code>h1</code> trebuie sa mosteneasca (inherit) fontul <code>monospace</code> de la elementul tau <code>body</code>.
    testString: assert(($("h1").length > 0 && $("h1").css("font-family").match(/monospace/i)));
  - text: Elementul tau <code>h1</code> trebuie sa mosteneasca (inherit) culoare verde (color green) de la elementul tau <code>body</code>.
    testString: assert(($("h1").length > 0 && $("h1").css("color") === "rgb(0, 128, 0)"));

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  body {
    background-color: black;
  }

</style>

```

</div>

</section>

## Solution
<section id='solution'>

```html
<style>
  body {
    background-color: black;
    font-family: monospace;
    color: green;
  }

</style>
<h1>Hello World!</h1>
```

</section>
