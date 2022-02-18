# Java Split 说明

---

```java
public class Split {

    public static void split1() {

        // \\s表示   空格,回车,换行等空白符,
        // +号表示一个或多个的意思\\s+表示已一个或多个空白为规则
        String s1 = "abc abc   ,   abca abc";
        String s2 = ", , , ,        a, eaefa";
        // 原因要分割出字符串中的空格，但是当空格个数多余一个时候
        // 就会默认分隔第一个，紧接后面的空格便会当成一个普通字符
        String [] str = s2.split(" ");
        for(String s : str)
        {
            System.out.println(s);
        }
        System.out.println("str数组的长度是:"+str.length);
    }

    public static void split2() {

        // \\s表示   空格,回车,换行等空白符,
        // +号表示一个或多个的意思\\s+表示已一个或多个空白为规则
        String s1 = "abc abc   ,   abca abc";
        String s2 = ", , , ,        a, eaefa";

        String [] str = s2.split("\\s+");
        for(String s : str)
        {
            System.out.println(s);
        }
        System.out.println("str数组的长度是:"+str.length);
    }

    public static void main(String[] args) {
        split1();
        System.out.println("========================");
        split2();
    }
}
```