### 1.What are the basic data types in TypeScript?
The basic data types in typescript are : 
1. Number 
2. string
3. Boolean
4. Any 
5. Array 
6. tuple  
7. unknown
### 2.What is Generic data type ?
TypeScript Generics is a tool which provides a way to create reusable components. It creates a component that can work with a variety of data types rather than a single data type. It allows users to consume these components and use their own types. Generics ensures that the program is flexible as well as scalable in the long term.

**Program :-**

> function identity(arg) {  
    return arg;  
}  
var output1 = identity("myString");  
var output2 = identity(100);  
console.log(output1);  
console.log(output2);

### 3.What is type inferring in TS?

TypeScript infers types of variables when there is no explicit information available in the form of type annotations.

Types are inferred by TypeScript compiler when:

a. Variables are initialized

b. Default values are set for parameters

c. Function return types are determined
### 4.What are the possible ways to define typing for functions?

In TypeScript, there are multiple syntaxes for declaring the type of a function:

1. Method signatures.
2. Function type literals.
3. Object type literals with call/construct signatures.

### 5.How to define Generic type for Classes?

TypeScript supports generic classes. The generic type parameter is specified in angle brackets after the name of the class. A generic class can have generic fields (member variables) or methods.

**program :-**

~~~ 
class chact={
   name: string,
   description: string,
   done: boolean
}
var todos:charct[] = [];
function add(name:string, description:string):charct[] {
 return todos.push({
 name: name,
 description: description,
 done: false
 });
 }
function remove(index) {
 return todos.splice(index, 1);
}
function list():void {
 todos.forEach(function(todo, index) {
 console.log(index + " - " + todo.name);
 });
}
function update(index:number, name:string, description:string):charct {
 todos[index].name = name;
 todos[index].description = description;
 return todos[index];
}