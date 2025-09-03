# Time complexity

### In this we will learn about time complexity for different algorithms.

We take example 
```
for (i=0;i<n; i++){ --> n+1
  statement --> n
}
```

>we don't need n+1 because it will not affect the degree

If i ask of order of algorithm then it is 

**O(n)**
Since this algorithm will run for n times 

Similarly,

```c
for (i=n;i>0; i-- ){
  statement
}
```

In this condition also the order remains 
O(n)

Similarly we can say,

```c
for (i=n;i<0; i+2 ){ 
  statement --> n/2
}
```

Here,

**f(n) = n/2**

But still order of n
**O(n)**

Now let's take another example to understand it better 

```c
for (i=0;i<n;i++){
  for (j=0;j<i;j++){
    statement;
  }
}
```

Let's trace this algorithm

i | j     | no of times(n)
--+-------+------------
0 | ~~0~~     | 0
--+-------+------------
1 |**0**,~~1~~    | 1
--+-------+------------
2 |**0**,**1**,~~2~~  | 2
**.  .       .**
**.  .       .**
**.  .       .**
**n          n**

And it continues  till n 
So if i ask you till how many times it is executed in total,
it will be

0+1+2+3+4+...no of times

Which can be written as 
f(n) = **∑(i=0 to n) i**

Which can represented as
f(n) = **n(n+1)/2** = **(n<sup>2</sup>+n)/2**

So the degree is 
O(n<sup>2</sup>)


Let's take another example,

```c
p = 0
for (i=1;p<= n; i++){
  p = p + 1;
}
```

Assumption, code will stop when `p>n`

Here,
p = k(k+1)/2
p = (k<sup>2</sup> + k)/2
p ~= k<sup>2</sup>

Loop will stop when 
k<sup>2</sup>>n
k>n<sup>1/2</sup>

So order is
O(n<sup>1/2</sup>)

### More examples

Let's take another algorithm and try to find the time complexity

```c
for (i=1;i<n;i=i*2){
  statement
} 
```


Let's analyze it 
```c
i     | values 
------+--------
2<sup>0</sup>*2     | 2 <sup>1</sup>
------+--------
2<sup>1</sup>*2     | 2 <sup>2</sup>
------+--------
2<sup>2</sup>*2     | 2 <sup>3</sup>
------+--------
```

