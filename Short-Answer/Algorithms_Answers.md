#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n * k) = The while loop might have been O(n) on it's own, the evulation needed to get the cube of n means depending on N's size the amount of inputs needed will grow. 


b) o(n^2) = The loop is trying to find when an exponentially growing number and a constantly growing number meet. Because it's loops are nested, while the input increases, the exponential J will grow at a larger and larger rate, making the inputs needed for the linear graph to meet it higher and higher. 


c) O(n) it's just getting called recursivly n times until it reaches it's base case.

## Exercise II
# A binary search makes the most sense to solve this problem..

# first you define some function that takes in an array
def egg_saver(arr):

# Then you would define low,mid, and high values setting them respectively with mid starting at 0
low = 0
high = len(arr) - 1
mid = 0

# create a while loop that waits for low and high to meet with a comparison like "<="
while low <= high:

# write an if to check if the egg breaks at mid, if it does it means we don't need to check any lower and move to the right
if break(mid) is True:
    low = mid + 1

# write an else to move to the left side otherwise and check there
else:
    high = mid + 1

# return mid once loop is over
    return mid

# binary searches run in a runtime complexity of O(log(n))
