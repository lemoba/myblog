## 《剑指offer》题解

> 《剑指Offer》第二版所有题目，共76道题目    题目来源：[Acwing](https://www.acwing.com/problem/search/1/?csrfmiddlewaretoken=S5lzkLHkKv13snNnUJUOL5GoHelfgamZ8nZzpmpLKjDjzHawX6aSvM1bd9dMw6f2&search_content=%E5%89%91%E6%8C%87Offer)
>

## 😜[简单题]

#### 84. 求1+2+…+n

```c
class Solution {
public:
    int getSum(int n) {
        int res = n;
        n > 0 && (res += getSum(n - 1));
        return res;
    }
};
```



#### 83. 股票的最大利润

```c
class Solution {
public:
    int maxDiff(vector<int>& nums) {
        if (!nums.size()) return 0;
        int res = 0;
        for (int i = 0, minv = nums[0]; i < nums.size(); i++)
        {           
            res = max(res, nums[i] - minv);
            minv = min(minv, nums[i]);
        }
        return res;
    }
}
```



#### 82. 圆圈中最后剩下的数字



```c++

```

