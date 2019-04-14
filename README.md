# PROBLEM LINK:
[Contest](https://www.codechef.com/KJSC2019/problems/ATCH/)

**Author:** [Shivam Pawase](https://www.codechef.com/users/shivam_1708)  
**Tester:** [Rushang Gajjal](https://www.codechef.com/users/)  
**Editorialist:** [Sangram Desai](https://www.codechef.com/users/sangram123)

## DIFFICULTY:
EASY  
## PREREQUISITES:  
Maximum sum subarrays.

## PROBLEM:
find the maximum sum of subarray given an array of n length.

## EXPLANATION:
In this problem, we have been given an array of n length.  
Since we need the maximum sum of subarray we use the concept of presum, to not calculate again and again, and store the sum and index in a map.  
Now in the map we have sub array sum so we loop through the map and find the negative number which can be removed from the subarray to get maximum sum.

for example:

5  
1 2 3 -2 3 

we get
0 1 3 6 4 7
but if we remove -2 
we get
0 1 3 6 9

maximum sum as = 9

**Note**: The indices are managed accordingly, as the first entry in presume array is 0.

**Part1:** get presum array.  
**Part2:** loop through the map and remove negative number.


## AUTHOR'S AND TESTER'S SOLUTIONS:  
Author's solution can be found [here](https://github.com/KJSCE-Codecell/Contests/blob/master/KJCS2018/Books/setter.cpp)  
Tester's solution can be found [here](https://github.com/KJSCE-Codecell/Contests/blob/master/KJCS2018/Books/tester.py)
