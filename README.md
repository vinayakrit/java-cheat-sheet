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
 
 
 
