# Java中split函数

#硬记

---





```java
public static void main(String\[\] args) {  
     
 //    "a\\b\\c" '\\'  a,b,c  
 String test \= "a\\\\b\\\\cd";  

 //  "a\\b\\c"    "\\"    a,b,c  
 String\[\] arr \= test.split("\\\\\\\\"); //    \\\\\\\\    \\\\   \\  
 for(String str : arr) {  
      System.out.println(str);  
   }  
}

```

split函数中\\ 表示转义, 又表示正则  
前两个表示为一个, 后两个表示为一个  
又表示正则, 两个斜线化为一个斜线

- [[打印目录结构]]