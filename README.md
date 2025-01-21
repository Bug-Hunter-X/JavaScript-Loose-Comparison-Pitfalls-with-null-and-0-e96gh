# JavaScript Loose Comparison Pitfalls with null and 0

This repository demonstrates a common JavaScript bug related to loose comparison (==) when dealing with null and 0.  Loose comparison can lead to unexpected results, especially when comparing numbers and null or undefined values. 

## Bug Description

The `foo` function aims to categorize numbers into negative, zero, and positive.  However, the loose comparison `x == null` incorrectly evaluates to `true` when `x` is 0. This results in incorrect categorization of 0 as 0 instead of 1.

## Bug Solution

The solution uses strict comparison (===) to correctly identify the value of x, avoiding the pitfalls of loose comparison.