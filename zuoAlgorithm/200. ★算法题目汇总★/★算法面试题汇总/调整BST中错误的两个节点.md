# 调整BST中错误的两个节点


#BST 

---
一棵二叉树原本是搜索二叉树，但是其中有两个节点调换了位置，使得这棵二叉树不再 是搜索二叉树，请找到这两个错误节点并返回。 已知二叉树中所有节点的值都不一样，给定二叉树的头节点 head，返回一个长度为2的 二叉树节点类型的数组errs，errs[0]表示一个错误节点， errs[1]表示另一个错误节 点。  

进阶: 如果在原问题中得到了这两个错误节点，我们当然可以通过交换两个节点的节点值的方 式让整棵二叉树重新成为搜索二叉树。 但现在要求你不能这么做，而是在结构上完全交换两个节点的位置，请实现调整的函数
