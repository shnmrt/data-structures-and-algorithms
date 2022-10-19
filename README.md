# data structures and algorithms
> lectures on the [patika.dev](www.patika.dev)

<img src="https://global-uploads.webflow.com/6097e0eca1e87557da031fef/609859a191abe5d64b17fed3_Patika%20logo-p-500.png" height='300'>

---
# Project 1
> Sort the given array by using ***insertion sort***

The insertion sort algorithm works by checking the rest of the array for to find the minimum value to replace it with current index.

## 1) What is the sort steps of this sorting algorithm
| State of array | Search index | Explanation |
|:----| :---: | ---: |
| [22,27,16,2,18,6] | - | Given array |
| [2,27,16,22,18,6] | 0 | change the location of the 22 and 2 in the array for index 0 
| [2,6,16,22,18,27] | 1 | change the location of the 27 and 6 in the array for index 1 
| [2,6,16,22,18,27] | 2 | the is no need to change the 16 because it already in the sorted form
| [2,6,16,18,22,27] | 3 | change the location of the 22 and 18 in the array for index 3 
| [2,6,16,18,22,27] | 4 | the is no need to change the 22 because it already in the sorted form
| [2,6,16,18,22,27] | 5 | the is no need to change the 27 because it already in the sorted form

## 2) What is the Big-O notation
O(n<sup>2</sup>)

## 3) Time complexity:

* Average Case : O(n)
* Best Case : O(n)
* Worst Case : O(n<sup>2</sup>)

## 4) What case does the number 18 fall into after the array is sorted?
Following the sort the number 18 is neither in head nor in tail, so it fall into ***average case***


## 5) What are the first four step of the given array regarding the insertion sort?
| Array | step | explanation |
| :---- | ---- | ----------: |
| [7,3,5,8,2,9,4,15,6] | Given | origin |
| [2,3,5,8,7,9,4,15,6] | 1<sup>st</sup> step | change the location of 7 and 2 |
| [2,3,5,8,7,9,4,15,6] | 2<sup>nd</sup> step | there is no need to change number 3 |
| [2,3,4,8,7,9,5,15,6] | 3<sup>rd</sup> step | change the location of 5 and 4 |
| [2,3,4,5,7,9,8,15,6] | 4<sup>th</sup> step |  change the location of 8 and 5 |

---
# Project 2
> Sort the given array by using ***merge sort*** 

Given array is [16,21,11,8,12,22]

## 1) Write down the step of the given array regarding the merge sort
[16,21,11,8,12,22]

[16,21,11] [8,12,22]

[16,21] [11] [8,12] [22]

[16] [21] [11] [8] [12] [22]

[16,21] [8,11] [12,22] 

[8,11,16,21] [12,22]

[8,11,12,16,21,22]

## 2) What is the Big-O notation?
O(n) -> nlogn

---
# Project 3

### Write down the binary-search-tree steps of the given array.

> Given array is [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

let the first element of the given array is root

                7
              /   \
            5       8
          /   \      \      
         1     6      9
        / \
       0   3
          / \
         2   4