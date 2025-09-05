# What are Algorithms?

## Algorithms vs Program 

We start coding with writing the approach first also called the pseudocode.

**Algorithms** are written during Design time.

**Programs** are written during implementation.

## Priori Analysis vs Posteriori Testing

### Priori Analysis
- Algorithms
- Independent of language
- Hardware Independent
- Time and space function

### Posteriori Testing
- Program 
- Language dependent
- Hardware dependent
- Watch time and Bytes

## Characteristics of Algorithm

- **Input**
 - 0 or more
- **Output**
  - Atleast 1 Output
- **Definniteness**
  -Everything should be logical
- **Finiteness**
  - It should stop somewhere
- **Effectiveness**
 - It should be logical

## How to write an Algorithm?
```
Algorithm swap(a,b)
Begin
  temp = a;
  a = b;
  b = temp;
end
```

## How to analyze an Algorithms
- Time
- Space
- Data Transfer over network
- Power 
- CPU registers

>Time and Space are main ones 

## Time Analysis

Every **simple** statement in Algorithm takes one unit of time.

Suppose the previous example

```
Algorithm swap(a,b)
Begin
  temp = a;  //1 unit of time
  a = b;  //1 unit of time
  b = temp;  //1 unit of time
end
```

So here f(n) = 3
This is a constant function of time.

Usually we represent them as 
O(1)
>order of one

Each sentence we say takes one unit of time exactly.
>this is our consideration

`temp = a`
`x = 5*a+6*b`

>In both the cases we say it takes one unit of time which is a under statement. The sentence is not appropriate if we go in detail because `x = 5*a+6*b` has one assignment and four arithmetics.


## Space Analysis

Every variable used is considered as unit of space.

```
Algorithm swap(a,b)
Begin
  temp = a;  //1 unit of space
  a = b;  //1 unit of space
  b = temp;  //1 unit of space
end
```

S(n) = 3
This is a constant function of space.
Each sentence we say takes one unit of time exactly.
>this is our consideration

Usually we represent them as 
O(1)
>order of one


