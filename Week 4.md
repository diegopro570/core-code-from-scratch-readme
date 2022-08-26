## Square(n) Sum

In this exercise we are going to introduce Typescript for the first time, we have to sum every square of every number inside the array:

```
export function squareSum(numbers: number[]): number {
    return numbers.reduce((item,n) => item + n*n,0)
}
```
