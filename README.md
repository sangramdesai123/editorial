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
In this problem, we have been given the number of pages in each book and the range of pages which makes a student like that particular book.  
Since we need the total number of pages we use the concept of presum, to not calculate again and again, and binary search since the order of books doesn't matter here.  
We sort the list of a number of pages for each book and calculate the presum for the sorted array. Now we apply binary search in order to find the position of li and ri for each student in this sorted list. Binary search can be implemented using bisect in python, and upper and lower bounds in C++. The difference of the indices returned for li and ri searches, will give you the number of books. And the difference of values in the presum array for the corresponding indices will give the total number of pages.

**Note**: The indices are managed accordingly, as the first entry in presume array is 0.

**Part1:** get presum array.  
**Part2:** binary search to get left and right index, and hence find the number of pages and books accordingly.


## AUTHOR'S AND TESTER'S SOLUTIONS:  
Author's solution can be found [here](https://github.com/KJSCE-Codecell/Contests/blob/master/KJCS2018/Books/setter.cpp)  
Tester's solution can be found [here](https://github.com/KJSCE-Codecell/Contests/blob/master/KJCS2018/Books/tester.py)
