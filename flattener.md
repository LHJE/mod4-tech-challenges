# Problem - Array Flattener
![recursion](https://media.giphy.com/media/3GuP496Wrkos8/giphy.gif)

Imagine you have a deeply nested array, or multi-dimensional array, like this:

```rb
 array_of_ints = [1, 2, 3, [[4], 5], [[[6]]]]]
 array_of_strings = ["hi", "this is", [[["string"], "that is very"], [[[["nested"]]]]]]
```
the contents of the array aren't important.

In Ruby and JS, we have built in methods and functions to `flatten` arrays into one dimension.  For example, in Ruby:

```rb
=> [1, 2, 3, [[4], 5], [[[6]]]]
[8] pry(main)> array_of_ints.flatten
=> [1, 2, 3, 4, 5, 6]
```
and in JS:

```js
> arr1
[ 0, 1, 2, [ 3, 4 ] ]
> arr1.flat()
[ 0, 1, 2, 3, 4 ]
```
If we look at the docs for either of these, we notice that they are _recursive_ by nature. Your goal is to recreate this functionality by writing a recursive function to accomplish this same thing. For example:

```rb
 array_of_ints = [1, 2, 3, [[4], 5], [[[6]]]]]
=> [1, 2, 3, [[4], 5], [[[6]]]]]
ruby_flattener(array_of_ints)
=> [1, 2, 3, 4, 5, 6]
```
or in JS:

```js
> arr1
  [ 0, 1, 2, [ 3, 4 ] ]
> flatten(arr1)
  [ 0, 1, 2, 3, 4 ]
```

# Instructions

1. Copy this markdown and paste in your own, privte gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom


## Rewrite the question in your own words:  
Recreate the recursive, built in `.flatten` method, taking a heavily nested array such as `[1, 2, 3, [[4], 5], [[[6]]]]` and returning `[1, 2, 3, 4, 5, 6]`.


## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?  
My first assumption is that, because this is a built in method, that this is a diffuicult (or at least annoying/tedious) task that is nonetheless incredibly useful.  I assume there will be recursion in this method, if only because it practically says so in the prompt, and that there will be conditionals somewhere in the method.

## What are your initial thoughts about this problem? (high level design, 2-3 sentences)  
It will be recursive.  There will be conditionals (maybe even something like `if "element".class == Array`).  It will take in an array and return a flattened array, without using the `.flatten` method.

## How would you identify the elements of this problem?

- [x] Searching of Data
- [x] Sorting of Data
- [ ] Pattern Recognition
- [ ] Build/Navigate a Grid
- [ ] Math
- [ ] Language API knowledge
- [ ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?  
Frankly I'm not sure if "Searching/Sorting of Data" is the right word for it, but out of those options I'd say they're the closest.  Likely no need for API, Math, or Grid stuff, but mayyybe pattern recognition?  Depending on what that means?

## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

def array_flattener(array)
 new_array that elements might be shoveled into?
 iterate over the array
  if conditional asking if this is an array?
   (this is where the recusive part is.  Maybe this iteration thing can be a helper method?  or the if conditional?  Let's get some real code going now)
  else
   shovel the element into the new array
  end conditional
 end iteration


 return the new_array
end


## Write out any implementation code OR link to repl  
Here it is!  It's not quite working, but I feel like I'm on my way to something...
[https://github.com/LHJE/flatten](https://github.com/LHJE/flatten)

## What is the Big O complexity of your solution?
oh, probably O^n
