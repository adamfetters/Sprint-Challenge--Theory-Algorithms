# Exercise 1

a) The amount of times ran will be equivalent of (n _ n / n).
Example if n = 5. 5 _ 5* 5 = 125. If you add 5 * 5 (25) to a, it will only be 5 runs until a is greater than the conditional. If you do 10 _ 10 _ 10 (1000) , you will add 10 \* 10 (100) to a each time and get 10 steps before the condition is met. So it seems that doubling n, therefore doubles the number of steps. The run time is linear in that it grows in direct proportion to what N is.

b) This is a logarithmic as dividing by 2 is increased as the number grows. If you start with 4, and i is divided by 2, 4 /2 = 2 / 2 = 1, you will have 2 steps until the condition is met. If you increased the number to 12, 12 /2 = 6 / 2 = 3 / 2 = 1, you then have only 3 steps. So as the number of n was multiplied x 3, the amount of steps only grew by a small amount.

c)This is also logarithmic or O(Log n). As the number increases the number of steps only increases by a small amount, or inversely proportional.

d)THis is O(n). As the number grows larger it is linear in time complexity.

e) O(n)2. As N grows the number of steps grows exponentially.

f) O(n);

g) O(n);

Exercise II
a) int firstHighest = array[0], int secondHighest=array[1], temp;
if (firstHighest < secondHighest) {
temp = firstHighest;
secondHighest = firstHighest;
firstHighest = temp;
}

for (int i = 2; i < array.length; i++) {
if (array[i] > firstHighest) {
temp = firstHighest;
firstHighest = array[i];
secondHighest = temp;

} else (if array[i] > secondHighest) {
secondHighest = array[i]
}
}

b) My strategy would be to pick the middle floor of the building and drop an egg. If the egg broke, I would then divide the lower half of the floors and drop an egg from the middle of that floor. If the egg didn't break, I would then divide the upper floors and drop an egg from the middle of that floor. I would continue this process until I found the floor from which it didn't break.

Exercise III

a) If it is already sorted and we start at the first index, then the running time is (O log n). This is the best case scenario for the quick sort algorithm, it will move up the array in order and keep everything where it is. It still has to check to make sure the values that are less than are put to the left of the pivot, so as the size grows it will take only partially longer as the array grows, but not that much.

b)Well best case scenario it will be (O log n), and worst case scenario will be (On^2). What determines the time complexity is how unbalanced it is to start with. If the tree is unbalanced the recurvise action needed will spend all it's time balancing the algo to the left, until it finally gets to the other side. On average it will be (O log n) because as the array grows, it will take less and less time to check partitions.
