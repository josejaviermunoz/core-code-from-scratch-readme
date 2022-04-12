# core-code-from-scratch-readme

[Week 1 Link](core-code-from-scratch-readme/Week1.md/ "Week 1 Link")

# Week 1

## Tuesday:

### Interpreted And Compiled Programming Languages:

**Interpreted Programming Lenguages:** 
```
Interpreted programming lenguage is run by the machine as it is excecuted. 
```
**Compiled Programming Lenguages:** 
```
Compiles programming lenguge is transformed to “machine lenguage” before it is excecuted.
```
### Is Java compiled or interpreted, or both?
```
Java is both, which in mortal terms means that it is compiled in a 2 step process: 

1. Compiled to bytecode.
2. Executed by a Java Virtual Machine. 

Modern Java technology compiles in real time as it is ran.
```
### **Pseudocode currency converter**

**Available Instructions:**
```
- Starting point: START
- Input: READ, GET
- Output: PRINT
- Math: +, -, *, /
- Assignation: <--
- Initialize: SET, INIT
- Add one: INCREMENT
- End point: END
```
**Currency convertor:**
```
1. START
2. Bitcoin <-- 39626.80
3. AmountUSD <-- GET
4. Var <-- AmountUSD / Bitcoin 
5. PRINT Var Bitcoin
6. END
```
## Wednesday:

**Your team has just seen the movie "Matrix" and you have been asked, how the number of your year of birth would be written in binary. You must learn how to translate your date of birth into binary and show your team.**
```
Date of birth: September 10, 1998
- 10 —> 1010
- 09 —> 1001
- 1998 —> 11111001110
```
**MIPS exercise**  
**Create a program that adds any two given numbers provided by the user**
```
.data
	      number1: .asciiz "\nIngrese el primer numero: "
	      number2: .asciiz "\nIngrese el segundo numero: "
	      result_message: .asciiz "\nThe result of the sum of the 2 numbers you gave is: "
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
              la $a0 result_message
              syscall

              li $v0, 1
              move $a0, $t2
              syscall
 ```            
**Create a program that displays your name**
```
.data
	      result_message: .asciiz "\nMy name is Jose "
  .text
	      main:

              li $v0, 4
              la $a0 result_message
              syscall
```
