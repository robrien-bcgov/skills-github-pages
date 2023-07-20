---
title: Welcome to my blog
---

## This is a H2 heading

* point 1
* point 2
* point 3

1. numbered list 1
2. 2
3. 3
4. 4

### block quote
> Most good programmers do programming not because they expect to get paid or get adulation by the public, but because it is fun to program. – Linus Torvalds


## definition of Done

Done
:  The definition of done (DoD) is when all conditions, or acceptance criteria, that a software product must satisfy are met and ready to be accepted by a user, customer, team, or consuming system.  We must meet the definition of done to ensure quality.  It lowers rework, by preventing user stories that don’t meet the definition from being promoted to higher level environments. It will prevent features that don’t meet the definition from being delivered to the customer or user.

### code for a reduce function (left reduce)
```javascript
const reduce = (reducer, initial, arr) => {
  let acc = initial;
  for (let i = 0, { length } = arr; i < length; i++) {
    acc = reducer(acc, arr[i]);
  }
  return acc;
};
```

### code for composing functions, e.g.: `y = f(g(x))`
```javascript
const compose = (...fns) => x => fns.reduceRight((y, f) => f(y), x);
```
