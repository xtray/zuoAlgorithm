# 一个数组中有一种数出现K次，其他数都出现了M次

---

一个数组中有一种数出现K次，其他数都出现了M次，
M > 1,  K < M
找到，出现了K次的数，
要求，额外空间复杂度O(1)，时间复杂度O(N)



```java

	// 请保证arr中，只有一种数出现了K次，其他数都出现了M次
	public static int onlyKTimes(int[] arr, int k, int m) {
		int[] t = new int[32];
		// t[0] 0位置的1出现了几个
		// t[i] i位置的1出现了几个
		for (int num : arr) {
			for (int i = 0; i <= 31; i++) {
				t[i] += (num >> i) & 1;
			}
		}
		int ans = 0;
		for (int i = 0; i < 32; i++) {
			if (t[i] % m == 0) {
				continue;
			}
			if (t[i] % m == k) {
				ans |= (1 << i);
			} else {
				return -1;
			}
		}
		if (ans == 0) {
			int count = 0;
			for (int num : arr) {
				if (num == 0) {
					count++;
				}
			}
			if (count != k) {
				return -1;
			}
		}
		return ans;
	}

```