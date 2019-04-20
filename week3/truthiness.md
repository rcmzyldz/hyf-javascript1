# Truthiness

Truthiness is very simple to understand.  Does a value convert to _true_ or _false_ when cast to boolean?

Paste this in the console to learn about truthiness, or study it [on python tutor](https://goo.gl/7tBTj3):
```js
{
  const x = ; // experiment with different values
  const truthiness_x = Boolean(x);

  if (truthiness_x) {
    console.log("truthy: " + typeof x + ", " + x);
  } else {
    console.log("falsey: " + typeof x + ", " + x);
  };
};
```
values to try:
```js
a: true       --> ?
a: false      --> ?
a: 0          --> ?
a: 1           --> ?
a: null       --> ?
a: undefined  --> ?
a: ''         --> ?
a: ' '        --> ?
a: 'tiil'     --> ?
a: 2          --> ?
a: 345        --> ?
a: NaN        --> ?
a: Infinity   --> ?
a: -Infinity  --> ?
a: -3         --> ?
a: -0.0       --> ?
```

This repo covers 4 important operators who's behavior is dependant on the _truthiness_ of their arguments.

### Index
* [falsey values](#falsey-values)
* [() ? : ;](#ternary-operator)
* [&&](#and-operator)
* [||](#or-operator)
* [!](#not-operator)
* [resources](#resources)


---
---

## Falsey Values

JavaScript has only 6 falsey primitive values.  All other values are truthy.

[on pytut](https://goo.gl/urDfWG)

```js
{
  const a = ;

  const truthiness = Boolean(a);

  console.log(typeof a + ", " + a + ", " + truthiness + "y");
};
```
the values:
```js
1: false      --> ?

2: null       --> ?

3: undefined  --> ?

4: ''         --> ?
4: ""         --> ?
4: ``         --> ?

5: NaN        --> ?

6: 0          --> ?
6: 0.0        --> ?
6: +0         --> ?
6: -0         --> ?
```


[TOP](#truthiness)

---

## Ternary Operator

The ternary operator evaluates the _truthiness_ of a value and returns either the first option or the second

[pytut link](https://goo.gl/xK4GcW)

Paste this in the console to learn about the ternary operator:
```js
{
  const x = ; // experiment with different values

  const coerce_truthiness = Boolean(x);
  const ternary_truthiness = (x) ? "truthy" : "falsey" ;

  const tern_option = (x) ? "first" : "second" ;
  const tern_numbers = (x) ? 1 : 2 ;
  const tern_boolean = (x) ? true : false ;

  console.log("x: " + typeof x + ", " + x);
  console.log("coerced: " + coerce_truthiness);
  console.log("ternaried: " + ternary_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("booleans: " + tern_boolean);
};
```
Ternary operators can only have two options.

values to try:
```js
a: true       --> ?
a: false      --> ?
a: 0          --> ?
a: 1          --> ?
a: null       --> ?
a: undefined  --> ?
a: ''         --> ?
a: ' '        --> ?
a: 'tiil'     --> ?
a: 2          --> ?
a: 345        --> ?
a: NaN        --> ?
a: Infinity   --> ?
a: -Infinity  --> ?
a: -3         --> ?
a: -0.0       --> ?
```


[TOP](#truthiness)

---

## And Operator

The and operator will return the first value if it's falsey, and the second value if the first is truthy.

[pytut link](https://goo.gl/G4mp9N)

Paste this in the console to learn about &&:
```js
{
  const a = ; // experiment with different values
  const b = ; // experiment with different values

  const and = a && b;
  const replication = (a) ? b : a ;

  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");

  console.log("and: " + and);
  console.log("replication: " + replication);
};
```
values to try:
```js
a: true, b:false      --> ?
a: false, b:true      --> ?
a: 0, b:1             --> ?
a: 1, b:0             --> ?
a: null, b:false      --> ?
a: false, b:null      --> ?
a: '', b:' '          --> ?
a: ' ', b:''          --> ?
a: 2, b:3             --> ?
a: 3, b:2             --> ?
```

[TOP](#truthiness)

---

## Or Operator

The or operator will return the first value if it's truthy, and the second value if the first is falsey.

[pytut link](https://goo.gl/gEztXo)

Paste this in the console to learn about ||:
```js
{
  const a = ; // experiment with different values
  const b = ; // experiment with different values

  const or = a || b;
  const replication = (a) ? a : b ;

  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");

  console.log("or: " + or);
  console.log("replication: " + replication);
};
```
values to try:
```js
a: true, b:false      --> ?
a: false, b:true      --> ?
a: 0, b:1             --> ?
a: 1, b:0             --> ?
a: null, b:false      --> ?
a: false, b:null      --> ?
a: '', b:' '          --> ?
a: ' ', b:''          --> ?
a: 2, b:3             --> ?
a: 3, b:2             --> ?
```

[TOP](#truthiness)

---

## Not Operator

The or operator will return the first value if it's truthy, and the second value if the first is falsey.

pytut links: [the snippet below](https://goo.gl/abjq1R), [! expanded](https://goo.gl/ej3y5j)

Paste this in the console to learn about !:
```js
{
  const a = ; // experiment with different values

  const not = !a;
  const coercion_replication = !Boolean(a);
  const ternary_replication = (a) ? false : true ;

  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("not operator: " + not);
  console.log("with coercion: " + coercion_replication);
  console.log("with ternary: " + ternary_replication);
};
```
values to try:
```js
a: true       --> ?
a: false      --> ?
a: 0          --> ?
a: 1          --> ?
a: null       --> ?
a: undefined  --> ?
a: ''         --> ?
a: ' '        --> ?
a: 'tiil'     --> ?
a: 2          --> ?
a: 345        --> ?
a: NaN        --> ?
a: Infinity   --> ?
a: -Infinity  --> ?
a: -3         --> ?
a: -0.0       --> ?
```

[TOP](#truthiness)

---

## Resources

__study tools__:
* [PythonTutor for JavaScript](http://pythontutor.com/javascript.html#)
* [the Parsonizer](https://janke-learning.github.io/parsonizer/)

__helpful links__:
* pytut snippets:
    * [truthy & falsey values](https://goo.gl/jBTLFD)
    * [&& vs. ||](https://goo.gl/BBXea6)
* [javascript.info](http://javascript.info/logical-operators)
* mdn: [logicals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operators), [ternary](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)
* [truthiness & comparisons](https://dorey.github.io/JavaScript-Equality-Table/) - click on the "if()" tab for truthiness
* from __boolean by example__:
    * [truthiness for the console](https://github.com/janke-learning/boolean-by-example/blob/master/README.md#truthiness)
    * [&&, || for the console](https://github.com/janke-learning/boolean-by-example#and-or-operators)
    * [! for the console](https://github.com/janke-learning/boolean-by-example#not)
    * [live in devtools](https://janke-learning.github.io/boolean-by-example/)
* mdn:
    * [boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean)
    * [truthy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)
    * [falsey](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)
* [a codepen](https://codepen.io/philipwalton/pen/nufrk)

[TOP](#truthiness)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
