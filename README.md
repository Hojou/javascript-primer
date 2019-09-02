# Angular Primer

This primer is meant as a _checklist_ for **you**.

This primer is **not about Angular** at all, it's about JavaScript and TypeScript (TypeScript being a superset of JavaScript). This is what we believe is fundamental knowledge about JavaScript/TypeScript; and knowing about these concepts is vital for understanding the upcoming Angular course. Most of this primer is about JavaScript, but a small section will adress TypeScript. The Angular course will be in TypeScript, but you will later see why that is not important right now.

It is advised to try and solve all the assignments (the BONUS ones are just for fun and if you're a nerd that likes to party - but are not required!). We have provided you with enough links to learn what is needed for each assignment. If you get stuck in an assignment, ask a buddy for help - that could be another intern or an employee.

Don't sweat it - we won't ask you for proof of completing the assignments (probably) - but it will make the course so much easier, since you can then concentrate on learning Angular and not basic JavaScript syntax.

## Basic weirdness

JavaScript looks like a lot of other object oriented languages, but it behaves differently in some cases. Using appropriate patterns and staying away from problematic structures can make JavaScript development easy though. We will try not to focus on stuff that probably won't be relevant for the course, but here is a few comparison examples that might seem weird :)

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators  
https://dorey.github.io/JavaScript-Equality-Table/

#### Assignments

```
  var funActivity = 'Solving problems';
  var doingActivity = 'true';
  var havingFun = true;
  var problem = undefined;
  var reference = null;
  var smallNumber = 0;
  var nextActivity = '';
  var wishList = [];
  var item = {};
```

Prove that all these statements are **true**, and understand why

- `!false`, `!!true`, `!!'false'`, `!item.funky`, `!wishList.length`
- `smallNumber == nextActivity`, `smallNumber !== nextActivity`
- `problem == reference`, `problem !== reference`
- `funActivity && havingFun`, `reference || havingFun`
- `wishList.length === 0`, `smallNumber === 0`

Prove that these statements are **false**, and understand why

- `!true`, `!'false'`, `!!item.funky`
- `funActivity !== havingFun`
- `problem === reference`, `problem != reference`
- `doingActivity === havingFun`, `doingActivity == havingFun`

**(BONUS)** What are the following expressions, and why

- `havingFun && funActivity`
- `doingActivity && funActivity`
- `item + wishList`
- `smallNumber + havingFun`

HINT: You can enter the expressions in the console of your favorite browser (Chrome - press F12)

## Functions

In JavaScript, functions are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called. In brief, they are Function objects.

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions

#### Assignments

1. Define or declare a named function
2. Define or declare an anonymous function
3. Define or declare an arrow functions
4. What are the benefits of the different function types. Why are there three different (basic) function types?
5. **(BONUS)** Explain what closure is, and why it is only awsome if you understand it
6. **(BONUS)** Explain what hoisting is
7. **(BONUS)** Define or declare a generator function

## Arrays

Arrays are high-level list-like objects. You recognize them from almost any other language. But refer to this link for more information:  
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

#### Assignments

```
const numbers = [1, 2, 3, 4, 5];
const persons = [{ name: 'Per' }, { name: 'Rasmus', funky: true }];
```

1. Use `map` and the array `numbers` to create a list like this: `[10, 20, 30, 40, 50]` (each number multiplied by 10)
2. Use `map` and the array `persons` to create a list like this: `['Per', 'Rasmus']` (the `name` property of each item)
3. use `filter` and the array `numbers` to create a list like this: `[3, 4, 5]` (all numbers equal to or more than 3)
4. use `filter` and the array `persons` to create a list like this `[{ name: 'Rasmus', funky: true }]` (all the funky persons)
5. use `filter` and `map` and the array `persons` to create a list like this `['Per']` (the name of all the persons that are not funky)
6. **(BONUS)** use `reduce` and the array `numbers` to calculate the sum 15.

#### Links

`.map` function: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map  
`.filter` function: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter

## TypeScript

TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. Without going into too much details, all you need to know for now is, that you can add type annotations and interfaces, as well as add attribute annotations to almost any object.

https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html

Since this is just a quick primer, here are a few key concepts to grasp:

- You `export` functions or variables in one file that you want to (re)use in another file.
- You `import` functions from other modules (files) that you want to use in your file.
- Use `let` to define variables that can be reassigned and `const` if they can not be reassigned.
- Any type can be declared or treated as `any` to _kind of_ bypass type checking. This is mostly not a good practice.

#### Links

https://www.typescriptlang.org/docs/handbook/modules.html  
https://www.typescriptlang.org/docs/handbook/module-resolution.html
