# Lists

![Difficulty](https://img.shields.io/badge/Difficulty-Medium-yellow)

## Problem

**Task**  
Given an integer, $n$, and $n$ space-separated integers as input, create a tuple, $t$, of those $n$ integers. Then compute and print the result of $hash(t)$.  

**Note:** [hash()](https://docs.python.org/3/library/functions.html#hash) is one of the functions in the `__builtins__` module, so it need not be imported.  

**Input Format**

The first line contains an integer, $n$, denoting the number of elements in the tuple.	 			
The second line contains $n$ space-separated integers describing the elements in tuple $t$.  

**Constraints**

 

**Output Format**

Print the result of $hash(t)$.

## Solution

**Language:** Python  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-30T17:27:56.575Z  

```py
if __name__ == '__main__':
    N = int(input())
    arr = []
    for i in range(N):
        command_input=input()
        cmdarr=command_input.split()
        if(cmdarr[0] == "insert"):
            arr.insert(int(cmdarr[1]),int(cmdarr[2]))
        elif(cmdarr[0]== "remove"):
            arr.remove(int(cmdarr[-1]))
        elif(cmdarr[0]== "append"):
            arr.append(int(cmdarr[-1]))
        elif(cmdarr[0]== "sort"):
            arr.sort()
        elif(cmdarr[0]== "pop"):
            arr.pop()
        elif(cmdarr[0]== "reverse"):
            arr.reverse()
        elif(cmdarr[0] == "print"):
            print(arr)
        else:
            print(arr)
        
                                                                                                                                                                             

```

---

[View on HackerRank](https://www.hackerrank.com/challenges/python-tuples/problem)