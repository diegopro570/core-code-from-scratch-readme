## Who likes it?

To give a brief introduction about how this works, it will take names on the argument of the function and will return wether who likes it or not.
```
let likes = names => {
    let factor = names.length
        if(factor==0){
            return "no one likes this"
        }
        else if(factor==1){
            return names[0]+" likes this"
        }
        else if(factor == 2){
            return names[0]+" and "+ names[1]+" like this"
        }
        else if(factor == 3){
            return names[0]+", "+names[1]+" and "+ names[2]+" like this"
        }
        else{
            return names[0]+", "+names[1]+" and "+(factor-2)+" others like this"
        }
    
}
```

## Bit Counting Exercise

This exercise consists in returning bits from a given decimal number, we have to implement a new method called **reduce()**, its function is to return a single value from an array
```
const countBits = (x) => {
  let test = x.toString(2).split("");
  let neuw = [];
  for (let i = 0; i < test.length; i++) {
    neuw.push(parseInt(test[i]));
  }

  let final = neuw.reduce((acc, item) => {
    return (acc = acc + item);
  });
  return final;
}
```

## Your Order, Please Exercise

In this exercise we are going to create a code that will sort a text where every single word has a number, it will display from the lowest one to the greatest one
```
const order = words => {

    let factor = words.split(" ")
    let neuw = []

    for(let i=0;i<=factor.length;i++){
        for(let j=0;j<factor.length;j++){
            if(factor[j].indexOf(i)>= 0){
                neuw.push(factor[j])
            }
        }
    }
    return neuw.join(" ")
}   
```

