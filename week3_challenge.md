# Problem - The Snail
![Snail](https://media.giphy.com/media/n17GyE4DbZfbO/giphy.gif)
Given an n x n array, write a method that returns the array elements arranged from outermost elements to the middle element, traveling clockwise.

A good way to visualize this is to picture the spiral shell of a snail! 

## JS Example
```js
const arrayMatrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
];

snail(arrayMatrix) #=> [1, 2, 3, 6, 9, 8, 7, 4, 5]
```

## Ruby Example
```rb
arrayMatrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
];

snail(arrayMatrix) #=> [1, 2, 3, 6, 9, 8, 7, 4, 5]
```

# Instructions

1. Copy this markdown and paste in your own, private gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom

Do not publish your code on a public repl.it or repo or other public means.

## Rewrite the question in your own words:

Write a method that will take in an n x n array, and return the outer most path spiralling inwards, clockwise.  Example:

### Ruby Example
```rb
array = [
  [1, 2, 3, 4],
  [5, 6, 7, 8],
  [9, 10, 11, 12],
  [13, 14, 15, 16]
];

snail(array) #=> [1, 2, 3, 4, 8, 12, 16, 15, 14, 13, 9, 5, 6, 7, 11, 10]
```

## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?
There may be some iterating that occurs.  There also may be some conditionals, and some measuring of length upon which those conditionals will be based.  Maybe some looping.  I assume these things because we're dealing with an array, and because that array does not have a fixed size.

## What are your initial thoughts about this problem? (high level design, 2-3 sentences)
My initial thought is the same as it always is: this problem is more complex than it at first appears.  Next: that I can likely start by getting my method to work on an array-matrix that is 3 x 3, and then once it's working there, see if I can expand it to work with a 4 x 4, and finally see if I can get it to work for Any size.

## How would you identify the elements of this problem?

- [ ] Searching of Data
- [ ] Sorting of Data
- [x] Pattern Recognition
- [ ] Build/Navigate a Grid
- [ ] Math
- [ ] Language API knowledge
- [ ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?
I don't think any Real math will be happening, beyond, I guess, counting.  And building a grid, once again, just seems like overkill (maybe if I practice at making a few, that won't seem like all that ridiculous of a prospect).  I can't really see much in there other than pattern recognition.  Maybe Sorting/Searching for data?  But that might be stretching the confines of those words haha.

## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

- start the method (array)
- check to see the size of the array, assign to a VARIABLE that will be used to do sooomething with the conditional and/or the iteration
- have something like "`return_array = array[0]`", since the first elements in the array that will be returned are always going to be the first.  Later, elements will be shoveled in (likely).
  - Heck, you might even be able to pop `array[0]` out entirely, since it's never accessed again
- use the VARIABLE to ...?

- return the return_array
- end the method

## Write out any implementation code OR link to repl
[Here's as far as my repo got](https://github.com/LHJE/snail_path)

## What is the Big O complexity of your solution?
Maybe O(1)? Likely O(n).
