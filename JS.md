## JS

### A seperation of concerns
-HTML - content
-CSS - presentation
-JS - behavior

`document.write('Good afternoon!');`
-document = the document oject. This represents the whole web page.
- . = the member operator. This is how you specify methods and properties, known as members of that object.
-write = a method within the document object.
-'Good afternoon!' = a parameter within the write method.
- ; = closing the argument.

### Data Types
-strings = "some text" or 'some text'
-number = 40 or 100
-variable = way to store data. Described by var. For instance, var someWord = 'cool';
-boolean = TRUE or FALSE. Period.
-functions - encapsulate code for reuse.
-arrays - 
-objects -
-undefined

### Operators
Example: `10 + '10';`
-An example of type coercion. Will output `1010` On all ifs, force strong evaluation by using `===`.
-In 301, we're required to use `use strict;` which means if we don't use `===`, code won't run.
`'some ' + 'cool' + 'thing'`
-An example of concatenation
`var first = 'noah';`
`var last = 'rhodes';`
`console.log(first + ' ' + last);`
-An example of variable based concatenation

### Arrays
-Arrays are lists. They can contain literally any other data type.
-`var people = ['sam','sally','eric'];`

-you can pull data out of the above through `people[item position]`

`for(var i=0; i<people.length; i++){
    console.log (people[i]);
}

### Objects
```
var person = {
    name: 'brian',
    age: 34,
    profession: 'principal' 
}

//console.log(person.name); will return 'brian'`

var person {
    name: 'brian',
    isEmployed: true,
    age: 34,
    kids: ['riley','rosalie','reid'],
}

To get riley, `console.log(person.kids[0]);`

var person {
    name: 'brian',
    isEmployed: true,
    age: 34,
    kids: [{name:'riley'},{name:'rosalie'},{name:'reid'}],
}

//To get riley in the above object, `console.log(person.kids[0].name);`

`var people = ['stronk','schmitt','sam','sally','eric'];

function peoplePosition(name){
  for(var i=0; i<=people.length; i++){
      if(people[i] === name){
        console.log(name+' is at position '+ i);
        return i;
      }
  }
}

peoplePosition('eric');
//This will return the position eric is in.

var person = {
  name: 'brian',
  age: 34,
  profession: 'instructor',
  kids: [
    {name: 'riley', age: 11},
    {name: 'reid', age: 4},
    {name: 'rosalie', age: 1, favMovies:['toy story','bambi']},
  ]
}

console.log('rosalie\'s favorite movie: ', person.kids[2].favMovies[1]);
//This will return rosalie
```
