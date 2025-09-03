# Frequency count method

### We are trying to find the time and space complexity.


This algorithm is used to find sum of elements in an array.
## Algorithm

```c
Algorithm sum(A,n){
  s = 0;
  for (i=0;i<n;i++){
    s = s+A[i];
  }
  return s;
}
```

Suppose we take array
A = 80085
n = 5 //number of values

### Time complexity
We know in the code block, 

`s=0` --> 1unit

And in 

`for (i=0;i<n;i++)` --> n+1

`i=0` --> 1 unit

`i<n` --> n+1 unit

`i++` --> n unit

Since we are bothered about highest only so whole line has has time complexity as 
`n+1`

`s = s+A\[i\];` --> n unit

`return s;` --> 1 unit

Therefore, f(n) = 1+(n+1)+n+1
**f(n)= 2n+3**

And we can say the order is 
**O(n)**

### Space Complexity
A --> n
n --> 1
s --> 1
i --> 1
S(n) = n+3

And the order is  
**O(n)**


## Let's take another example

The following algorithm finds sum of two matrices (2D Arrays)

```c
Algorithm Add(A, B, n){
  for (i = 0; i < n; i++) {       --> n+1 
    for (j = 0; j < n; j++) {        --> n * (n+1)
      C[i][j] = A[i][j] + B[i][j];      --> n*n
    }
  }
}
```

### Time complexity
So we can say that the time complexity is 

**f(n) = 2n<sup>2</sup> + 2n + 1**

And the order is 
**O(n<sup>2</sup>)**

### Space complexity 
A = n<sup>2</sup>
B = n<sup>2</sup>
C = n<sup>2</sup>
n = 1
i = 1
j = 1

S(n) = 3n<sup>2</sup> + 3

And degree is 
O(n<sup>2</sup>))

