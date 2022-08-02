## Multiply Exercise

From a given code that does not execute properly we have to find a typo on syntax so that the code will execute correctly:
```
function multiply(a, b){
  a * b
}
```
so as we could see it is a function that actually is not returning any information after it executes, so to fix this code we only have to add a return statement and that will be it!
```
function multiply(a, b){
  return  a * b
}
```

## ASCII Exercise

For this exercise we are going to use an encoding format to translate a sentence into numbers, also we are going to use a new function called **charCodeAt()** that specifically does the task for this exercise:
```
function uniTotal (st) {
    let cont=0;
    let str = new String(st);

    for(let i=0;i<st.length;i++){
        cont += str.charCodeAt(i);
    }
return cont;
}
``` 
so if we execute the function
```
console.log(uniTotal("aaa"));
```
it will display on the console 291 which is exactly ASCII format

## Char From ASCII Value Exercise

this exercise on the opposite to the previous one, from a given number we have to return the ASCII value also we are going to use a new method which is **String.fromCharCode()** so the code will be:

```
function getChar(c){
  return String.fromCharCode(c)
}
```
so it was simple right? in this case the string is not a primitive, it is an object also it has to be used like that because this method is static so it means that we do not need to create an object prior we execute it.

## Binary Addition Exercise

In this exercise from two decimal numbers we have to sum both numbers so that we are going to return the total in binary. In this exercise we are going to use the method **toString()** so the code will be:

```
function addBinary(a,b) {
  return (a+b).toString(2)
}
```
what I like of this method is that it is versatil, we used the binary system so we had to add 2 inside the parentheses but if we would have wanted to use the hexadecimal system we had to type 16 inside the paretheses so on. It is an amazing method, is not it?.

## Student´s Final Test Exercise

We need to create a function that returns:

- 100, if a grade for the exam is more than 90 or if a number of completed projects more than 10.
- 90, if a grade for the exam is more than 75 and if a number of completed projects is minimum 5.
- 75, if a grade for the exam is more than 50 and if a number of completed projects is minimum 2.
- 0, in other cases

so I am going to use decion-maker statements as **if** and **else if** also I am going to use logical operators as **&&** (AND), **||** (OR).

```
function finalGrade(exam, projects) {
  if (exam > 90 || projects > 10) {
    return 100;
  } else if (exam > 75 && projects >= 5) {
    return 90;
  } else if (exam > 50 && projects >= 2) {
    return 75;
  } else {
    return 0;
  }
}
```
## Remove All Exclamation Marks From The End Of Sentence

In this exercise we are going to apply a new method **replace** so the code will be:

```
let remove = str =>{
    return str.replace(/!+$/g,"")
}
```
To explain the first argument better the ""+"" symbol means that the function has to include all the elements that we are looking for, the **$** sign means that it will only take the element at the end and the whole argument is called **literal notation**.

## Vowel Remover Exercise

In this exercise as the previous one we are going to use the **replace()** method so the code will be:
```
let shortcut = str =>{
    return str.replace(/[aeiou]/g,"")
}
```
we can also use arrays as literal notation.

## Rock Paper Scissors!

In this exercise we are just going to use decision-maker statemets and logical operator so the code will be:
```
let game = ["scissors","rock","paper"]
    if((p1===game[0] && p2===game[1])||(p1===game[1] && p2===game[2])||(p1===game[2] && p2===game[0])){
        return "Player 2 won!"
    }
    else if((p2===game[0] && p1===game[1])||(p2===game[1] && p1===game[2])||(p2===game[2] && p1===game[0])){
        return "Player 1 won!"
    }
    else if(p1===p2){
        return "Draw!"
    }
    else{
        return null
    }
```
## Persistent Bugger Exercise

This exercise consists in returning the number of times that we have to multiply digit by digit of x number until getting just one digit, we are going to use a new method called **split()** that separates a text-string taking a separaror as argument, also we will use the method **toString()** that tranforms any object into a string.

```
let persistence = num =>{
    let factor = num.toString().split("")
    
    while(factor.length>1){
        let result = 1
        for(let i=0;i<factor.length;i++){
            result=result*factor[i]
        }
        factor=result.toString().split("")
    }
    return factor
}
```

