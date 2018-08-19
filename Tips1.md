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
s + ESC //delete current character and change to insert mode and adding space + space  
; //repeat f+ 
. // repeat the second steps

##### Tips7. Pause with the brush off your page

很简单，当你停下来编辑的时候请按ESC回到normal mode下,通常来说我们退出insert mode的情况下都是在最后的位置，所以一个简单的做法就是当我们想再次输入的时候 敲击A，来到句尾

或者创建新的一行o来编写

##### Tips9 Compose Repeatable Change

举一个例子，删除一个单词，我们就应该用daw = "delete a word",这样的好处是可以我们要再删除一个单词可以直接用.


##### Tips10 Use Count to do the Simple Arithmetic
C-a 如果在数字上，就相当于加法，如果cursor不在数字上，想到与cursor jump to 第一个数字上
C-x,如果在数字上，相当于减法，如果cursor不在数字上，相当于调到第一个数字上

