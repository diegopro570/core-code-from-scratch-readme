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

## Playing with digits

```
const digPow = (n: number, p: number) => {
  let numero: string[] = n.toString().split("");
  let realNumbers: number[] = numero.map(Number);
  let total: number = 0;

  for (let i = 0; i < realNumbers.length; i++) {
    total = total + realNumbers[i] ** p;
    p++;
  }
  if (total >= n && total % n == 0) {
    let bucle: number = total;
    let counter: number = -1;
    while (bucle >= 0) {
      bucle = bucle - n;
      counter++;
    }

    return counter + " " + total;
  } else {
    return -1;
  }
};
```

