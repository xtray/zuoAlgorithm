# N个数字有多少种进出栈的方式
#卡特兰数 

---

N 个数字, 进N 个数出N 个数。问你有多少种进出栈的方式。

---

就是括号问题吗？进栈是左括号，出栈是右括号，有多种进栈的方式就在任何时候  
任何一个前缀上右括号数量不能比左括号要多，就是合法的进出站方式, 就是卡特兰数