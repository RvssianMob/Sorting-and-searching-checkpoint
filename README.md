# Sorting-and-searching-checkpoint
Insertion Sort Checkpoint

This repository contains a solution to the Insertion Sort, which is a classic sorting algorithm that works by iterating through an array and inserting each element into the correct position in the sorted portion of the array. The solution is implemented in JavaScript and includes a function called insertionSort that takes an array as input and returns the sorted array.

Features
1. Efficient and simple implementation of the Insertion Sort algorithm in JavaScript

2. Uses two counters to iterate through the unsorted and sorted portions of the array

Usage
To use the insertionSort function, simply call it with an array of integers as input. The function will return a sorted array in ascending order.

JavaScript.

function insertionSort(arr) {
  for (let i = 1; i < arr.length; i++) {
    let key = arr[i];
    let j = i - 1;
    while (j >= 0 && arr[j] > key) {
      arr[j + 1] = arr[j];
      j--;
    }
    arr[j + 1] = key;
  }
  return arr;
}

// Example
let arr = [5, 2, 4, 6, 1, 3];
let sortedArr = insertionSort(arr);
console.log(sortedArr);


Installation
To install the Insertion Sort, simply clone the repository to your local machine and run the index.html file in your web browser. The code is written in JavaScript and does not require any additional dependencies.
