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
-arrays
-objects
-undefined

### Operators
- `=` the assignment operator
- `+` addition. Can also be used in strings to concatenate values.
- `-` subtraction.
- `/` division.
- `*` multiplication.
- `++` increment. Adds one to the current variable, e.g. i++
- `--` decrement. Subtracts one to the current value, e.g. i--
- `%` modulus. divides two values and returns the remainder. 10 % 3 = 1, as 10/3 = 3 remainder 1.
*Order of operations applies*

### Variables
-Declared by using `var`
-Can be declared in groups, e.g `var a, b, c`

#### 6 rules for assigning variable names
1. Must begin with a letter, dollar sign or underscore. Variables cannot start with a number.
2. Variable names cannot use periods, dashes (-), as these are operators.
3. Variables cannot use reserved words. See the full list of reserved words here: http://javascriptbook.com/extras/keywords-and-reserved-words/
4. Variables are case sensitive. However, it is bad practice to create two variables with the same name for different cases.
5. Try to be descriptive but brief in your variable names. firstName is obviously a variable meant for a first name, ect.
6. camelCase is your friend. It will make sure you don't screw things up.

### Arrays
-Arrays are lists. They can contain literally any other data type.
-`var people = ['sam','sally','eric'];`

-you can pull data out of the above through `people[item position]`

for(var i=0; i<people.length; i++){
    console.log (people[i]);
}
The above will output every person in the people array



### Objects

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

