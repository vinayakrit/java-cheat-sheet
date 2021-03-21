# java-cheat-sheet


## Increment & decrement 

   ```java
    int a=5;
    a++; 
   ``` 
   > This will increase value of 'a' after end of statement by 1
   
   ```java
   int a=5;
   ++a;
   ```
   > This will increase value of 'a' at the end of statement by 1

> if first condition true in a condition statement, next condition are ot checked 

```java
if(condition_1 || condition_2)
```
> here if condition _condition_1_ true then condition _condition_2_ will not checked.
> And if not true then _condition_2_ will be checked.
###### Note : even if condition statement is false/true statement is compiled. Suppose we have conditional statement if(System.out.println("Hello") == null) "Hello" will be printed
  

Let take a simple example where first cindition is true
  ```java
  int a=5;
  if(++a==6 || a++==6)
  System.out.println(a);
  ```
  >So here when we use pre-increment on _a_ it become _6_ & so _6==6_ will true hence post-increment of _a_ i.e _a++==6_ ignored and at time of printing it prints _6_ rather than printing _7_
  
 Let take a simple example where first cindition is false so we will check second condition 
 ```java
  int a=5;
  if(a++==6 || a++==6)
  System.out.println(a);
  ```
  >So here first condition _a++==6_ is false so we moved to second condition but our value increased because we ended with first condition statement now second condition is true and our output will printed as _7_
 
 
 ## Casting 
 ```java
   a=+b;  
 ```
 > a = (int) (a + b)

###### Integer/doubles to character
```java
char ch = (char) 65.65;
```
> Simply this will cast double value to char as per ASCII which is _A_


###### Character to integer
```java
int i = (int) 'A';
```
> Simply this will cast character _A_ to inetger as per ASCII which is 65


###### Integer to string
```java
int number = 456;
String str = number + "";
```
>This will change integer to string 


###### String to integer
```java
String str = "456";
int number = Integer.parseInt(str);
```
> This will parse string "456" to an integer value 456

 
## Something about Characters in java

iCheck whether character is type of digit or not
```java
Character.isDigit('9');
```
Or
```java
char ch = '9';
Character.isDigit(ch);
```
>This will return boolean _true_ if ch is digit of character else return _false_

Here are others

Syntax | meaning
------------ | -------------
Character.isLetter(ch); |  return boolean _true_ if ch is letter of character else return _false_
Character.isLetterOrDigit(ch); | return boolean _true_ if ch is letter or digit of character else return _false_
Character.isLowerCase(ch); | return _true_ if character ch is lower case else _false_
Character.isUpperCase(ch); | return _true_ if character ch is upper case else _false_
Character.toLowerCase(ch); | return lower case of character ch
Character.toUpperCase(ch); | return upper case of character ch


