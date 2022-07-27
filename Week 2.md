# Multiply Exercise

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

# ASCII Exercise

For this exercise we are going to use an encoding format to translate a sentence into numbers, also we are going to use a new function called charCodeAt() that specifically does the task for this exercise:
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
