## Square(n) Sum

In this exercise we are going to introduce Typescript for the first time, we have to sum every square of every number inside the array:

```
function squareSum(numbers: number[]): number {
    return numbers.reduce((item,n) => item + n*n,0)
}
```

## A wolf in sheep's clothing

```
function warnTheSheep(queue: string[]): string {
  
    let total = queue.reverse().indexOf('wolf')

    if(total == 0){
        return "Pls go away and stop eating my sheep"
    }else{
        return "Oi! Sheep number "+total+"! You are about to be eaten by a wolf!"
    }
  
}
``` 
