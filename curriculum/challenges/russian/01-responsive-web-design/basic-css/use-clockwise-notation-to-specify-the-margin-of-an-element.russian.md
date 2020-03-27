---
id: bad87fee1348bd9afdf08726
title: Use Clockwise Notation to Specify the Margin of an Element
challengeType: 0
videoUrl: https://scrimba.com/c/cnpybAd
forumTopicId: 18345
localeTitle: Используйте обозначение по часовой стрелке, чтобы указать маржу элемента
---

## Description
<section id='description'>
Давайте попробуем это снова, но с <code>margin</code> в этот раз. Вместо того, чтобы указывать свойства <code>margin-top</code> , <code>margin-right</code> , <code>margin-bottom</code> и <code>margin-left</code> отдельно, вы можете указать их все в одной строке, например: <code>margin: 10px 20px 10px 20px;</code> Эти четыре значения работают как часы: верхний, правый, нижний, левый и будут давать тот же результат, что и при использовании отдельных margin свойств.
</section>

## Instructions
<section id='instructions'>
Используйте <code>Clockwise Notation</code> чтобы дать элементу класса <code>blue-box</code> margin <code>40px</code> на его верхней и левой сторонах, и только 20 <code>20px</code> на нижней и правой стороне.
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Clasa <code>blue-box</code> trebuie sa le atribuie elementelor <code>40px</code> de <code>margin</code> in partea de sus (top).
    testString: assert($(".blue-box").css("margin-top") === "40px");
  - text: Clasa <code>blue-box</code> trebuie sa le atribuie elementelor <code>20px</code> de <code>margin</code> in partea dreapta (right).
    testString: assert($(".blue-box").css("margin-right") === "20px");
  - text: Clasa <code>blue-box</code> trebuie sa le atribuie elementelor <code>20px</code> de <code>margin</code> in partea de jos (bottom).
    testString: assert($(".blue-box").css("margin-bottom") === "20px");
  - text: Clasa <code>blue-box</code> trebuie sa le atribuie elementelor <code>40px</code> de <code>margin</code> in partea stanga (left).
    testString: assert($(".blue-box").css("margin-left") === "40px");
  - text: Trebuie sa folosesti notatia dupa acele ceasornicului (clockwise notation) pentru a seta marginile clasei <code>blue-box</code>.
    testString: const removeCssComments = str => str.replace(/\/\*[\s\S]+?\*\//g, '');assert(/\.blue-box\s*{[\s\S]*margin[\s]*:\s*\d+px\s+\d+px\s+\d+px\s+\d+px(;\s*[^}]+\s*}|;?\s*})/.test(removeCssComments($('style').text())));

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .injected-text {
    margin-bottom: -25px;
    text-align: center;
  }

  .box {
    border-style: solid;
    border-color: black;
    border-width: 5px;
    text-align: center;
  }

  .yellow-box {
    background-color: yellow;
    padding: 20px 40px 20px 40px;
  }

  .red-box {
    background-color: crimson;
    color: #fff;
    margin: 20px 40px 20px 40px;
  }

  .blue-box {
    background-color: blue;
    color: #fff;
  }
</style>
<h5 class="injected-text">margin</h5>

<div class="box yellow-box">
  <h5 class="box red-box">padding</h5>
  <h5 class="box blue-box">padding</h5>
</div>

```

</div>

</section>

## Solution
<section id='solution'>

```html
<style>
  .injected-text {
    margin-bottom: -25px;
    text-align: center;
  }

  .box {
    border-style: solid;
    border-color: black;
    border-width: 5px;
    text-align: center;
  }

  .yellow-box {
    background-color: yellow;
    padding: 20px 40px 20px 40px;
  }

  .red-box {
    background-color: crimson;
    color: #fff;
    margin: 20px 40px 20px 40px;
  }

  .blue-box {
    background-color: blue;
    color: #fff;
    margin: 40px 20px 20px 40px;
  }
</style>
<h5 class="injected-text">margin</h5>

<div class="box yellow-box">
  <h5 class="box red-box">padding</h5>
  <h5 class="box blue-box">padding</h5>
</div>
```

</section>
