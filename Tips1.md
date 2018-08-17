### Tips1 Meet The Dot Command

Line One
Line Two
Line Three
Line Four

##### Our Goal: 
Delete One Line and Delete Two lines

In general, 
For first Goal 
we can use _x_ to delete character and use _.._to Restore the change;

Second Goal:
We can press  _dd_ to delete whole line and use . to repeat several times.


##### Conclude
```jshelllanguage
-> dd //remove whole line
-> . //repeat last action
-> >G //increase the indentation till end of the File
-> u //revert last change  
```


### Tips 2 Don't Repeat YourSelf

var foo 1;
var bar = 'a';
var foobar = foo + bar;

##### Our Goal
Adding the semicolon at the end of every line

Method 1 : -> a;ESC j$. j$. //, save a;ESC
Method 2 : -> A;ESC j. j. //. save A;ESC change j$a;ESC to jA;ESC

##### Conclusion 

```jshelllanguage

-> A //append to the end of the line no matter where is the cursor 
```


### Tip3 Take one Step back, Then Free Forward

var foo = "method(" + argument1 + "," + argument2 + ")";

##### Our Goal 
Adding space before and after + 

##### Steps

1. f+
2. s + ESC
3. ;
4. .
5. ;.
6. ;. 

Explain:
f+ //move the cursor to the first appearance 
s + ESC // delete current character and change to insert mode and adding space + space  
; //repeat f+ 
. // repeat the second steps


