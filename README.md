Short List
==========
- [Coding Challenge 1 - Java Coder](#coding-challenge-1---java-coder)
___________

## Coding Challenge 1 - Java Coder
**Java Code -**
```java
public class CodeXam{
    public static void main(String [] arr){
     Integer num1 = 100, num2 = 100, num3 = 500, num4 = 500;
        if(num3 == num4 ) {
            System.out.println("3");
        }else if(num1 == num2) {
            System.out.println("4");
        }else{
            System.out.println("2");
        }
    }
}
```
**Output -**
```
4
```
**Explanation -**
The output is 4 because the value of num1 and num2 are equal to 100 and the value of num3 and num4 are equal to 500. So, the output is 4 even num3 and num4 are equal to 500 but if we store it in int then the output will be 3.
