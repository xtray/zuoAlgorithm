# Java中split函数

#硬记

---
ref: https://m.runoob.com/java/java-string-split.html

split() 方法根据匹配给定的正则表达式来拆分字符串。
注意： . 、 $、 | 和 * 等转义字符，必须得加 `\\`。
注意：多个分隔符，可以用 | 作为连字符。

split函数中  `\\` 表示转义, 如果按`\`切分, 需要写成`split("\\\\")`

```java
String[] words = article.split("\\s+"); // NOTE: 多个空格的切分技巧
```


```java
public static void main(String[] args) {  
  
    // "a\b\c"  
    String test = "a\\b\\c"; // 两个斜杠表示一个斜杠本身  
  
    // "a\b\c" 按斜杠切分, \ 是转义字符, 所以前面得加\\
    String[] arr = test.split("\\\\");  
    // String[] arr = test.split("\\\\", 2); // 分割为 a  b\c 两组  
    for (String str : arr) {  
        System.out.println(str);  
    }  
}

```


- [[打印目录结构]]