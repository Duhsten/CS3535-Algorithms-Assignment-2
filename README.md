# CS 3535 ALGORITHMS - Assignment 2: Angular Sorting and Closest Pair of Points

## Introduction

In this assignment, we explore two algorithms: Angular Sorting with Timsort and Closest Pair of Points. Angular Sorting with Timsort is a sorting algorithm that sorts points based on their angle relative to a pivot point, and it is used to solve the convex hull problem in computational geometry. Closest Pair of Points is a problem of finding the two closest points among a set of points on a 2D plane.

## Angular Sorting with Timsort

The algorithm for Angular Sorting with Timsort involves sorting the points based on their angle relative to a pivot point. We first select the leftmost point as the pivot point and calculate the angle between this point and every other point in the set. We then sort the points based on their angles using Timsort, a hybrid sorting algorithm that combines merge sort and insertion sort. Once the points are sorted, we can apply Graham's scan algorithm to compute the convex hull of the set.

## Closest Pair of Points

The algorithm for Closest Pair of Points involves sweeping two lines across a set of points on a 2D plane, while maintaining and querying several data structures. We sort all the points based on the x-coordinate and scan two lines i and j across the point set from left to right. Every time line j advances to a new point pj, line i advances to a point pi such that the difference between the x-coordinates of pj and pi is at most the current minimum distance D. We store all the relevant points in a binary search tree keyed on the y-coordinate, and query this data structure to find all points close to pj. We iterate through all the successors (and predecessors) until we reach a point beyond the relevant box. If a closer pair is found, the minimum distance D is updated. This algorithm has a worst-case time complexity of O(n log n).

## Skills Gained

Through this assignment, we gained the following skills:
- Understanding of Angular Sorting with Timsort
- Familiarity with the Closest Pair of Points algorithm
- Ability to implement algorithms in computational geometry

## Acknowledgments
This assignment was completed as part of the CS 3535 ALGORITHMS course offered by Appalachian State University. The assignment description was provided by Dr. Raghuveer Mohan who was inspired by Dr Brian C. Dean.
