---
layout: post
title: What I Learned Yesterday - "This" is confusing
---

*Every day at AcademicWorks, the Engineering Team has a Dev Sync where we share something we learned from the day before. Often times we'll hear about some new movie, a cool Kickstarter project, or an interesting ruby gem. Our VP of Engineering has issued a challenge to our team: Whoever can teach something they learned from the day before that is 1) technical in nature and 2) directly related to our work for 20 consecutive days will win a prize. Here is what I learned yesterday...*

# In Javascript, `this` is confusing

`this` is a special variable in Javascript because its available everywhere.

It can be used in: 

- functions
- outside functions (in the top-level scope)
- in a string passed to `eval()`

## What I learned

One of the benefits to using **strict mode** in javascript is that if you make a mistake using `this`, strict mode assigns `this` to `undefined` instead of the global object (`window` in the browser).

### Example pitfall
- If you forget the keyword `new` when invoking a constructor function, `this` could be assigned to the global object if you were in "sloppy mode".



##More reading: 
- [JavaScript’s “this”: how it works, where it can trip you up](http://www.2ality.com/2014/05/this.html)