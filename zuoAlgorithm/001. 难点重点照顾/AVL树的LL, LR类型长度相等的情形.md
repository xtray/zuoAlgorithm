# AVL树的LL, LR类型长度相等的情形

---


明显是LL型的, 右旋总是对的  
LR型跟LL型, 明确告诉你是哪一种, 就做相应的调整就行了  

相等的时候认为是LL一定合理, 但是不能认为是LR型  
![[Pasted image 20201218012955.png|500]]


LR型跟LL型, 有明确的长度不同, 就做相应的调整就行了  
如果发现, 左边的左树跟右树长度一样, ==必须只做LL型调整==

![[Pasted image 20201218113157.png|600]]

![[Pasted image 20201218113211.png|400]]