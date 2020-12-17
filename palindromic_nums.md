# Problem - Palindromic Numbers
![Palindrome](https://media.giphy.com/media/xT5LMYqyIPJtjnjiHm/giphy.gif)

The number 47 has an interesting characteristic.

If you take the number, plus its reverse (47 => 74) and then add them together to a number (47+74=121) the resulting sum is a palindrome

Starting at 0, find the first 25 numbers that have this same characteristic as 47, but limit it to where the palindrome is greater than 1000.

Collect the results in an array. Be sure that you're collecting the interesting numbers like 47, not the palindromic sums.

Bonus points if you can do this without converting numbers to strings/arrays.

Limit your online searches to core language documentation only.

# Instructions

1. Copy this markdown and paste in your own, private gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom


## Rewrite the question in your own words:

Starting at 0, put into an array the first 25 numbers that when added to it's reverse, the sum is a palindrome.  Example: 47 + 74 = 121.  However, limit these numbers to those whose palindrome some is greater than 1000.  Example: 1234 + 4321 = 5555.  Bonus points if you don't convert the numbers into another datatype.


## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?

I assume:
- I will have to create an Array of ?? number of ascending numbers, and iterate over them.
- I will in a refactor make it so that once a number has been tested, that it's reverse is removed from the array, as it has already been tested.
- I will be doing rudimentary math
- I will have a conditional
- I will be shoveling in numbers that are part of the array I'm iterating over into another array, which will be returned.
- I will likely start off by making the number strings, even though there are bonus points for not doing it that way.  That can be changed in a refactor.
- I might be able to start the array at 109 instead of 0, because no number below 109 when added to it's reverse is above 1000.  I can likely refactor it to start at the first number that ends up having a palindrome sum, since 109, 119, 129 ... 199 all don't result in a palindrome sum.


## What are your initial thoughts about this problem? (high level design, 2-3 sentences)
The liklihood that the numbers will grow ever larger the more numbers being asked for is high.  Which means the conditional will have to be very clever indeed.  The method will take in the limit of numbers, it will make an array of, I still don't know how long, and will end once the new array has 25 entries into it.

## How would you identify the elements of this problem?

- [x] Searching of Data
- [ ] Sorting of Data
- [x] Pattern Recognition
- [ ] Build/Navigate a Grid
- [x] Math
- [ ] Language API knowledge
- [ ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?
Likely there will be a pattern that emerges, but I'm not sure what that is until I see what sort of numbers actually do have palindrome sums with their reverse.  So to start out with, it'll likely be simple math and searching of data.

## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

def get_palindromes(length of final array)  
  - making an empty array to eventually return aka return_array  
  - line of code that allows me to iterate over an infinite array of sequential numbers starting with 109.  
    - conditional asking if return_array has 25 entries, if so:  
      - break  
    - elsif stating that if the number added to its reverse equals a palindrome, then:  
      - shovel that number into the return_array  
    - else  
      - next  
    - end  
  - end  
  - return return_array  
end  

## Write out any implementation code OR link to repl

[https://github.com/LHJE/palindrome](https://github.com/LHJE/palindrome)

## What is the Big O complexity of your solution?
If my pseudocode is any indication, O(n).  But who knows when I get in there.
