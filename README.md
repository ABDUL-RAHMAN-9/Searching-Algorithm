# Searching-Algorithm
<p>
  Searching algorithms are essential tools in computer science used to locate specific items within a collection of data. These algorithms are designed to efficiently navigate through data structures to find the desired information, making them fundamental in various applications such as databases, web search engines, and more.
  
</p>

<h2>Linear Search Algorithm</h2>
<p>Given an array, arr of n integers, and an integer element x, find whether element x is present in the array. Return the index of the first occurrence of x in the array, or -1 if it doesn’t exist.</p>

```
Input: arr[] = [1, 2, 3, 4], x = 3
Output: 2
Explanation: There is one test case with array as [1, 2, 3 4] and element to be searched as 3. Since 3 is present at index 2, the output is 2.


Input: arr[] = [10, 8, 30, 4, 5], x = 5
Output: 4
Explanation: For array [10, 8, 30, 4, 5], the element to be searched is 5 and it is at index 4. So, the output is 4.


Input: arr[] = [10, 8, 30], x = 6
Output: -1
Explanation: The element to be searched is 6 and its not present, so we return -1.
```

<h2>Program:</h2>

```
#include <iostream>
#include <vector>
using namespace std;

int search(vector<int>& arr, int x) {
    for (int i = 0; i < arr.size(); i++)
        if (arr[i] == x)
            return i;
    return -1;
}

int main() {
    vector<int> arr = {2, 3, 4, 10, 40};
    int x = 10;
    int res = search(arr, x);
    if (res == -1)
       cout << "Not Present";
    else
       cout << "Present at Index " << res;
    return 0;
}
```

<h2>Output:</h2>
<br>

```
Present at Index 3
```

<h2>Time Complexity:</h2>
<br>

```
Worst Case: O(N)
Auxiliary Space: O(1) 
```
