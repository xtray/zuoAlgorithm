# Manacher算法

#Manacher算法

---

- 题目1: [[最长回文子串的长度]]
- 题目2: [[字符串变为回文需要添加的最少字符]]


暴力解:  
就是你每个你把处理上的每一个位置将左右两边扩出去得到最大值除 2 就是原始串中最长回文子串的长度


## Manacher算法核心
1）理解回文半径数组  
2）理解所有中心的回文最右边界R，和取得R时的中心点C  
3）理解   L…(i')…C…(i)…R  的结构，以及根据i'回文长度进行的状况划分  
4）每一种情况划分，都可以加速求解i回文半径的过程  

- [[Manacher算法代码]]




