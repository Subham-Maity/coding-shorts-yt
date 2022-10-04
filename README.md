Short List
==========
- [**Coding Challenge 1 - Java Coder**](#coding-challenge-1---java-coder)
- [**Coding Challenge 2 - Python & Java Coder**](#coding-challenge-2---python--java-coder)
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

## Coding Challenge 2 - Python & Java Coder
**Java Code -**
```java
public class CodeXam{
    public static void main(String[]args){
        int CodeXam = 0x000F;
        int Xam = 0x57;
        System.out.println(CodeXam & Xam);
    }
}
```
**Output -**
```
7
```
**Python Code -** 
```python
CodeXam = 0x000F
Xam = 0x57
print(CodeXam & Xam)

```
**Output -**
```
7
```
**Explanation -**
0x000F - 15
0x57 - 87 
15 in binary is 0000 1111
87 in binary is 0101 0111
**We know, and operator will return 1 if both the bits are 1 else it will return 0.
So, 0000 1111 & 0101 0111 = 0000 0111 = 7 in decimal.**



