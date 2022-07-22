## Interpreted And Compiled Programming Languages
### Compiled Laguanges
They are the ones that take the sytax from the programmer and translate the syntax into machine code creating a new file ready to be executed and when this code has a new change the whole code has to be compiled again, these kind of laguages are usually faster and more efficient than interpreted languages because we can say the process is direct. One disadvantage is that compiled languages are not multi-platform some examples could be C++, C, Go etc.

### Interpreted Languages
They are the ones that are run by a text editor and executed line by line so they are more dinamic in the way of making changes on the program but as this process seems diligent they are less efficient and slower to compiled languages. One advantage can be they are multi-platform some examples could be Javascript, Python, Ruby etc.

## Is Java Compiled, Interpreted Or Both?

This is a good question because there are not only two types of programming languages, there is one more that are called hybrid laguages and Java is one of them, in this case Java compiles the code through the Java compiler to get bytecode and the JVM (Java Virtual Machine) executes it, but there is also an implementation of JVM that interprets the code instead of compiling it.

## Pseudocode Currency Converter
The next code converts dollars into bitcoins:


```
1. START 
2. Bitcoin <-- 0.000043 (bitcoin value on 20/07/2022 4:00 PM CST)
3. Dollars <-- GET
4. x <-- Bitcoin*Dollars
5. PRINT x
6. END
```
## My Year Of Birth In Binary

I was born in 2000 so lets check a set of positions that will help us to find 2000 in binary:

|position|binary|
|--|---|
|0|2^0 = 1|
|1|2^1 = 2|
|2|2^2 = 4|
|3|2^3 = 8|
|4|2^4 = 16|
|5|2^5 = 32|
|6|2^6 = 64|
|7|2^7 = 128|
|8|2^8 = 256|
|9|2^9 = 512|
|10|2^10 = 1024|

If we pick position 4, 6, 7, 8, 9 and 10 the sum will give us 2000 so my year of birth in binary is **11111010000**

## MIPS Exercises

first of this is a low-level language, the first exercise consists in getting 2 numbers and display the sum: 

```
.data
	      number1: .asciiz "\nType in first number: "
	      number2: .asciiz "\nType in second number: "
	      result: .asciiz "\nThe sum is "
  .text
	      main:
              li $v0, 4
              la $a0, number1
              syscall

              li $v0, 5
              syscall

              move $t0, $v0

              li $v0, 4
              la $a0, number2
              syscall

              li $v0, 5
              syscall

              move $t1, $v0
              
              add $t2, $t0, $t1
              
              li $v0, 4
              la $a0, result
              syscall

              li $v0, 1
              move $a0, $t2
              syscall
```

The second exercise consists in displaying a name: 
```
 .data
	      name: .asciiz "\nDiego\n"
  .text
	      main:
              li $v0, 4
              la $a0, name
              syscall
```
## Print Special Numbers

The following section shows a code in JavaScript that displays all the even numbers form 0  to 100 using a flow control stucture, as my favorite one is "for" I am going to put it out in practice but it does not mean that it is the only flow control structure, we also have While, do while, for each etc.

```
for(let i= 0; i<=100; i+=2){
    console.log(i);
}
```

## Bad code

The following code has an error and our task is to find what the error is: 

```
var cond = false;

if ((cond = true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
```
As we can see on the third line inside the argument of the flow structure "if", the "=" is not a conditional, it is assigning a new value to **cond** which is the value "true" but it does not make sense that we want to re-assing a variable inside an "if" so the right code will be: 

```
var cond = false;

if ((cond == true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
```

## Bad code 2

In this section we had to help a confused programmer that wanted to create a program with the following outputs:

1. If the number is 100 the system has to display **This is a special number!**
2. If the number is less than 1000, multiple of 10 and not equal to 100 the system has to display **This number is almost special**
3. If the number does not match with any instruction above the system has to display **Just a regular number**

so in JavaScript the final result will be:

```
let numbfunc=(litt)=>{

    let n=litt.toString();
    
    if(n == 100){
        console.log( "This is a special number!");
    }
    else if (n<1000 && n.endsWith(0) && n != 100 && n!=0){
        console.log("This number is almost special");
    }
    else{
        console.log("Just a regular number")
    }

}
```
