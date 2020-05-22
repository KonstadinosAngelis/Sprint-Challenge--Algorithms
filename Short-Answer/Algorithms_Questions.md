# Analysis of Algorithms

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```
O(n * k) = The while loop might have been O(n) on it's own, the evulation needed to get the cube of n means depending on N's size the amount of inputs needed will grow. 


```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
```
o(n^2) = The loop is trying to find when an exponentially growing number and a constantly growing number meet. Because it's loops are nested, while the input increases, the exponential J will grow at a larger and larger rate, making the inputs needed for the linear graph to meet it higher and higher. 

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```
O(n) it's just getting called recursivly n times until it reaches it's base case.


## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

What makes the most sense to minimize the amount of eggs broken is a binary search. 

#Define some function that takes an array
def egg_saver(arr): 

#Define some variables that will track our position in the array
low = 0
high = len(arr) - 1
mid = 0

#Create a while loop that will end once we've found our number
while low <= high:

    #Find the middle of the function
    mid = (high+low)//2'


    #Call the "check if breaking" function on the middle to see if it's our number
    if break(mid) is False:
    #we know we need to go lower if it doesn't break here
        high = mid + 1

    #if the egg is breaking at the mid level, we know we don't need to search any higher up

    #call it on the left side to see if it's there    
    elif break(mid) is True:
        low = mid + 1
    
    if it gets here we've found it
    else:
        return mid
    
