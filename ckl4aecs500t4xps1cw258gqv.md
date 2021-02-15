## Arrays Properties and methods in JavaScript

Arrays are the most common data structure used in development. This is the first thing that comes to our mind when we come across some sort of list. In this article, we'll explore **some** basics and **some** advanced concepts which will help us improve our understanding of arrays and the modern methods associated with arrays. so, without further ado let's jump into it.

let's start and brush up on the basics.

* So let's create an array first - 
 ** An array can contain any type of data, call it Numbers, Strings, Booleans, Objects, or even a mix of all of these.**

```javascript
const emptyArray = [];
const numbers = [1, 2, 3, 4, 5];
const houses = ['Gryffindor', 'Slytherin', 'Ravenclaw', 'Hufflepuff'];
const randomData = ['hello', 20, true, {name: "Nilesh", age:"21"}];


```

*  Accessing elements -  like most other languages JavaScript too follows 0-based indexing that means the first element is indexed 0.

```javascript
const names = ['John', 'Steve', 'Sara'];
console.log(names[0]); // output: John
console.log(names[2]); // output: Sara
```

*  let us now perform Inserting and overwriting using array index, if you escape any indices, by default those will be undefined. (See example in code below)


```javascript
names[3] = 'Robert';
console.log(names); 
// output: ['John', 'Steve', 'Sara', 'Robert']
names[2] = 'Thoda-sa'; // overwrites
// output: ['John', 'Steve', 'Thoda-sa', 'Robert']

names[6] = 'James';
console.log(name);
// output: ['John', 'Steve', 'Thoda-sa', 'Robert', undefined, undefined, 'James']


```

* push and unshift methods: push method adds an element at the end and unshift at the beginning.

```javascript
const numbers = [1, 2, 3, 4];
numbers.push(100);
console.log(numbers);
// output: [1, 2, 3, 4, 100]

numbers.unshift(-100);
console.log(numbers);
/// output: [-100, 1, 2, 3, 4, 100]

```

* pop and shift methods are used to delete elements, let's see them in action

``` javascript
const primes = [2, 3,  5, 7, 11, 13];
const deletedElementUsingPop = primes.pop();
console.log(primes);
// output: [2, 3, 5, 7, 11]
const deletedElementUsingShift = primes.shift();
console.log(primes);
// output: [3, 5, 7, 11]
console.log(deletedElementUsingPop); // output: 13
console.log(deletedElementUsingShift); // output:  2



```

* now let's see the length property(not a method) of an array

```
const brands = ['nike', 'addidas', 'supreme', 'Puma');
console.log(brands.length) // output: 4
```

## Strings and Arrays

* split and join are a few of the most important methods used to solve problems dealing with strings and arrays. let's see how these methods works - 

```javascript
const greeting = 'hello world';
const arr = greeting.split(' ');
console.log(arr);
// output: ['hello', 'world']

const newGreeting = arr.join('-');
console.log(newGreeting)
// output: 'hello-world'


```
### Now that we know how to deal with arrays,  Let us solve a problem : 
> problem : Reverse a String without reversing its single words.

```python
#  input: 'holmes sherlock is name the' 
#  output: 'the name is sherlock holmes'

```
Try to solve this on your own and come back to compare with mine


```javascript
const message = "holmes sherlock is name the";
const parts = message.split(" "); 
// ['holmes', 'sherlock', 'is', 'name', 'the']

let num = [];
while (parts.length > 0) {
  num.push(parts.pop());
}
// num = ['the', 'name', 'is', 'sherlock', 'holmes']

const answer = num.join(" ");
console.log(answer);
// output: 'the name is sherlock holmes'

```
Congratulations 🎊 , you made it to the end.
Thank you so much for stopping by, I hope you learned something from this. I'll see you next time.
<br> <br>
And yes, you can follow me here to get notified for my future posts,  'the name is @nileshhazra'.  Ciao!





