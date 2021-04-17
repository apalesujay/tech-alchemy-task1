# Tech Alchemy Assignment -Task 1
This repository contains the solution to Tech Alchemy Assignment - Task 1

## Problem Statement
You are a developer who accidently went back in time. You can’t return back to your timeline because you Time machine need to sort array from 10 Gigabytes of unsorted integer data. The problem in front of you is Machine during that time was not that advanced. You find a device with 1 gigs of ram and 240 Gigabyte of hard drive.

* They are all integers like 10000, 16723998 etc.
* Same integer values can be repeatedly appearing in the file.
Create a function to read 10 gigabytes of data and sort it. (Pseudo code and logic will also work)

## Solution
The solution to this problem can be divided into two phases:
* Sorting the multiple chunks of data
* Mergin the sorted chunks of data into a single large file.

Following steps to be followed to get the solution to the above problem statement:
1. Divide the large file into smaller chunks of data which will fit into the RAM of 1GB i.e. `size_of_each_chunk <= 1GB`.
2. Read the each chunk into memory.
3. Use merge sort to sort each chunk.
4. Store the sorted chunk of data on the hard drive.
5. Once all the chunks are sorted and stored on the hard drive, we can K-way Merge algorithm to merge the `n` sorted files into a single large sorted file.
6. Heap or Tournament Tree data structure can be used to perform K-way Merge.
7. The heap is more commonly used, although a Tournament Tree is faster in practice.
