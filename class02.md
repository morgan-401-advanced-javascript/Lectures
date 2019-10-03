# October 1st 2019

### Schema
Object that describes an object
EX:
`const schema = {
    fields: {
        id: {type: 'string', required: true},
        name: {type:'string', required: true},
        age: {type: number},

    }
}`

### !!
Can be used to convert data to a boolean and then return boolean
!1 = false -> !false -> true && !!1 = true
!!null = false && !!undefined = false && !!0 = false
Evaluates the "truthyness" of vague input and returns a defined boolean. 

### Vocab
#### Node,js
run js environment outside of the browser
#### Package
Everything you need to use a module
#### npm 
node package manager. Lets you install packages & run scripts
#### Unit test
test or group of test that fully covers a independent module or piece
#### TDD Test Driven Development
process where you write a test early in code process. and write small chunks that pass test. Encourages MODULAR coding. 
#### Modular

#### Functional Programming
make everything modular and use as many functions as possible instead of writing or re-writing custom code. 

### Lecture

#### Pure functions
use a variable without modifying the original && Immutable
Predictable give same arguement always return same result. Not unpredicatable 

#### ... Spread Operator
deep copies and puts in a new variable

#### Anonymous Functions
() => {}
ad hoc/ one-off logic
namesless usually set as an arguement, variable, or return value

### More Vocab!!
#### Object
instance, basic unit of data/code that we use. Can be a variable, data structure, a function, etc. Usually have a type that defines what kind of data & operations 
#### Class
template for a structure/type of an object. define what kind of data an object should hold and what kind of operations you can do on an object
#### Inheritance
Parent class gives things to a child/decendant
animal(has age) -> mammal -> dog(has bark & fur)   Animal has age & any specific dog will have age
new Dog has bark & fur + age
Allows us to reuse logic from a previously defined class & build
#### Class v2
use a constructor to initialize any object from that class. 

### Demo
class Animal {
    constructor(name, species){
        this.name = name;
        this.species = species;
    }
}

class Dog extends Animal {}

module.exports = Dog;

super() --my parents constructor

class Dog extends Animal {
    constructor(name){
        super(name, 'dog')
        this.name = name;
        // no longer req this.species = species;
    }
}
