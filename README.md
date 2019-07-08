# css-distribute-on-circle
Automatically distribute any amount of elements around a circle with css.

## Usage

### Using the sass mixin

HTML:
`<ul class='circle-container'>
  <li><img src='http://lorempixel.com/100/100/city'></li>
  <li><img src='http://lorempixel.com/100/100/nature'></li>
  <li><img src='http://lorempixel.com/100/100/abstract'></li>
  <li><img src='http://lorempixel.com/100/100/cats'></li>
  <li><img src='http://lorempixel.com/100/100/food'></li>
  <li><img src='http://lorempixel.com/100/100/animals'></li>
  <li><img src='http://lorempixel.com/100/100/business'></li>
  <li><img src='http://lorempixel.com/100/100/people'></li>
</ul>`

Sass:
`@import 'distribute-on-circle.scss';

.circle-container {
  @include distribute-on-circle(32, 20em, 6em);
  margin: 5em auto 0;
  border: solid 5px tomato;
}`

### Using the precompiled css
Simply import the css file with the maximum supported elements you need (files end in max-8, max-16, etc) and use the same html format as above.