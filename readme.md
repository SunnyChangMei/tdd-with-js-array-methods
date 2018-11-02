# Test Driven Development with Javascript Array Methods

I'm taking a test driven development approach to write my own version of javascript's array methods. I'm using a modified version of the javascript testing framework, [tinytest](https://github.com/joewalnes/tinytest), for my tests. A big thanks to Gordon Zhu's [Watch & Code](http://watchandcode.com) course for giving me a methodology I'm able to understand and use to put into practice.

## Instructions

You're welcome to play around with my code and tests.

1. Clone or download this repository
2. Open any of the HTML files within the *array-methods* directory in Chrome or browser of preference
3. Right-click inside the browser window and click *Inspect*
4. Click *Console*
5. Review the passing/failing tests

## Using the Debugger

You can add the debugger to any test to take a step by step look at the code.

For example, to add debugger to the first test of my findIndex method:

1. Open *forIndex.html* in your editor
2. Insert a new line after line 70 and paste in `debugger;`

```
'1. It should run the callback function originalArray.length number of times.': function() {
  debugger;
  var numberOfTimesCallbackHasRun = 0;
  var originalArray = [1,2,3];
  findIndex(originalArray, function(){
    numberOfTimesCallbackHasRun++
  });
  eq(numberOfTimesCallbackHasRun, 3);
},
```

### Methods to Test

#### Iterators:

- [x] Array.prototype.forEach()
- [x] Array.prototype.filter()
- [x] Array.prototype.map()
- [x] Array.prototype.reduce()
- [x] Array.prototype.find()
- [x] Array.prototype.findIndex()
- [ ] Array.prototype.every()
- [ ] Array.prototype.some()
- [ ] Array.prototype.reduceRight()

#### Accessors:

- [ ] Array.prototype.concat()
- [ ] Array.prototype.indexOf()
- [ ] Array.prototype.lastIndexOf()
- [ ] Array.prototype.includes()
- [ ] Array.prototype.slice()
- [ ] Array.prototype.join()

#### Mutators:

- [ ] Array.prototype.push()
- [ ] Array.prototype.pop()
- [ ] Array.prototype.shift()
- [ ] Array.prototype.unshift()
- [ ] Array.prototype.fill()
- [ ] Array.prototype.reverse()
- [ ] Array.prototype.copyWithin()
- [ ] Array.prototype.sort()
- [ ] Array.prototype.splice()
