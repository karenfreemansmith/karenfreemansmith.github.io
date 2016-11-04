# Typescript Notes

Typescript is a superset of JavaScript. It allows us to use ES6 features (*like strict typing and classes*) to write and debug our code, but compiles into regular (*ES5*) JavaScript.

## Helpful Links
* [Typescript in 30 Minutes](http://tutorialzine.com/2016/07/learn-typescript-in-30-minutes/)
* [TypeStrong Learn Typescript](https://github.com/TypeStrong/learn-typescript)
* [Treehouse Typescript Workshop](https://teamtreehouse.com/library/getting-started-with-typescript-2)

## Getting Started
* $ npm install typescript -g
* $ apm install atom-typescript (Optional, the add-on doesn't run well on my laptop - causes Atom to freeze up. It can also be installed through the ui under preferences/install)

## Basic Syntax (Hello World)
var greeting: string = "Hello World - from TypeScript!";
console.log(greeting);

## Running a Program
* $ tsc app/hello.ts (will compile the .ts file into .js of same name and in same folder)

## Type Declarations
* var variablename: type;
* var myString: string;
* var myArray: string[];
* var myNumber: number;

## Typescript Classes
```
class Greeter {
  greeting: string;

  constructor (message: string) {
    this.greeting = message;
  }

  greet() {
    return "Hello, " + this.greeting;
  }
}
```

Unlike JavaScript with it's prototypes, methods are declared inside the class as member functions. Each class requires a constructor.

## Typescript Loops
```
for(var thing of things) {
  console.log(thing);
};
```

(Pickup at "Inheritance")
