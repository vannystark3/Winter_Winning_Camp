# **2. Reverse a Number**

### Objective
 - Reverse the digits of a given number n. For example, if the input number is 12345, the output
should be 54321. The task involves using loops and modulus operators to extract the digits
and construct the reversed number.

### Task
 - Given an integer n, print the number with its digits in reverse order.
   
### Input Format
 - One integer n.

### Constraints
```
1≤n≤10^9
```

### Output Format
 - Print the number with its digits in reverse order.

## Test Cases
### Example 1:

**Input:**
```
12345
```
**Output:**
```
54321
```

**Explanation:**
```
The digits of 12345 in reverse order are 54321.
```
### Example 2:
**Input:**
```
9876
```
**Output:**
```
6789
```
**Explanation:**
```
The digits of 9876 in reverse order are 6789.
```
### Example 3:
**Input:**
```
1000
```
**Output:**
```
1
```
**Explanation:**
```
The digits of 1000 in reverse order are 0001, which is equivalent to 1.
```
## Solution
### Code (C++)
```cpp
#include <iostream>
using namespace std;
#define MAX 1000000000

int main() {
    int n,a,m=0;
    cout<<"Enter n : ";
    cin>>n;
    if(n>=1 && n<=MAX){
        while(n!=0){
        a = n%10;
        n = n/10;
        m = m*10+a;
        }
        cout<<"Reversed number : "<<m;
    }
    else{
        cout<<"Error : Input out of range!";
    }
    
    return 0;
}
```
## Output
### Test Case 1
  <picture>
    <img alt="" src="">
  </picture>

### Test Case 2
<picture>
    <img alt="" src="">
  </picture>

### Test Case 3
<picture>
    <img alt="" src="">
  </picture>
