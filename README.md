# Sell-Stock  ![image](https://github.com/user-attachments/assets/7cca53a1-6bcb-4375-a625-935b3565da3e)

This Python program is an implementation of the "Best Time to Buy and Sell Stock " problem, where we are given an array prices representing stock prices on different days and an integer k representing the maximum number of transactions allowed. The goal is to maximize the profit by making at most k buy-sell transactions.

Breakdown of the Code -
The solution consists of three main components:

1.MinMaxList function: 
This function reduces the given price array to only the peaks (sell points) and valleys (buy points).
How it works:
Iterates through the price array while keeping track of increasing and decreasing trends.
It filters out unnecessary price fluctuations, keeping only local minimums and maximums.
If the final length is odd, the last element is removed to maintain pairs of buy/sell points.


2.Double Linked List Implementation:
It allows efficient removal of transactions when needed.
Helps in merging buy/sell pairs efficiently.

3.Max Profit Calculation using MinHeap:(Uses a heap-based greedy approach to remove the least profitable transactions)-
step 1: Calls MinMaxList() to simplify the price list.
Step 2: Calculates the maximum profit without considering transaction limits.
Step 3: If the number of valid transactions (m) is already ≤ k, return the computed profit.
Uses a heap-based greedy approach to remove the least profitable transactions.

Time Complexity Analysis - O(nlogn)
This Problem is from #leetcode( DP )


