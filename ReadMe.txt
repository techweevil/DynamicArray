# Dynamic Array Problem

This is my solution to the Dynamic Array problem. It involves performing dynamic array operations based on a given set of queries.

## Problem Description

The problem requires implementing a dynamic array that supports two types of queries:

1. Query type 1: Appending an element to a specific sequence of the dynamic array.
2. Query type 2: Retrieving an element from a specific sequence of the dynamic array and updating the last answer.

## Solution

I have solved the problem by implementing the `dynamicArray` function. It takes the following parameters:
- `n`: the number of empty arrays to initialize.
- `queries`: a list of query strings that contain 3 space-separated integers.

The function returns an array with the results of each type 2 query in the order they are presented.

### Algorithm

1. Initialize an empty list of lists, `newArray`, with `n` empty lists.
2. Iterate over each query in `queries`.
    - If the query is of type 1, append the element to the corresponding sequence in `newArray`.
    - If the query is of type 2, retrieve the element from the corresponding sequence in `newArray` and update the last answer.
3. Return the list of last answers.

### Example Usage

```csharp
List<List<int>> queries = new List<List<int>>
{
    // Add your example queries here
};

List<int> result = dynamicArray(n, queries);
Console.WriteLine(string.Join(", ", result));
