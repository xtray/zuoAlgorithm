# Manacher算法

---

## [[Manacher算法]]
假设字符串str长度为N，想返回最长回文子串的长度

时间复杂度O(N)


## Manacher算法核心
1）理解回文半径数组  
2）理解所有中心的回文最右边界R，和取得R时的中心点C  
3）理解   L…(i')…C…(i)…R  的结构，以及根据i'回文长度进行的状况划分  
4）每一种情况划分，都可以加速求解i回文半径的过程  

## 题目
[[字符串变为回文需要添加的最少字符]]   
[[判断两个字符串是否互为旋转词|旋转字符串]]   
[[两棵二叉树是否有一致结构的子树]]   

