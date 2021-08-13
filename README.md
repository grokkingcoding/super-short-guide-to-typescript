![Image of Yaktocat](https://source.unsplash.com/sL2BRR1cuvM)

### About

- This is a short introduction to typescript and how we can use it in an application built with the popular frontend framework, ReactJS

- to git clone this repo, use: https://github.com/grokkingcoding/super-short-guide-to-typescript.git

### Super Short Guide To TS

1. To sump up the key benefit of ts is that it basically lets you the developer implement strict type checking in all your variables so as to avoid errors e.g. a variable that should always be an array being changed to an object. This would never happen with typescript.

2. So lets get right into an example. For exmaple, if we have a varibale that we used typescript to make it of type string then it would look something like this (let userID: string;).

```
let userID: string;

userID = '12345'

userID = 12345

```

What do you think will happen in the above code? Yes, there will be an error when we try to do userID = 12345 because 12345 is a number whereas userID should be strictly type stirng. The TS compiler will pick up on this error and notify us.

3. In javascript a variable can also be a function like this:

```
const someCoolFunction = (somethingCool) => {
    return somethingCool;
};
```

So how do we type check a function? Like this:

```
const someCoolFunction = (somethingCool: string): string => {
    return somethingCool;
};
```

A shorter version can be written like this:

const someCoolFunction = (somethingCool: string): string => somethingCool;

For numbers, we do something like this:

```
const subtract = (x: number, y: number): number => x - y;
```

Why do we need to do type check after the parentheses you may ask? The ": number" after the parentheses are type checking the return value from the funciton.

4. So how does TS become JS? The TS is transpiled into JS so when during JS runtime there is no typescript present.

5. Remember that TS is a development tool and no TS exist after it has been transpiled into JS.

6. How about if we have two or more argument in the function? In cases like these we can apply type check to each of the arguments passed in.

7. Can we do optional arguments in TS? Yes, but there may be an issue can you think of it?
