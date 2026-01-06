# B2144 阿克曼（Ackermann）函数

## 题目描述

阿克曼（Ackermann）函数 $A(m,n)$ 中，$m, n$ 定义域是非负整数（$m \le 3$，$n \le 10$），函数值定义为：

$\mathit{A}(m,n)=n+1$；（$m=0$ 时）。

$\mathit{A}(m,n)=\mathit{A}(m-1,1)$；（$m>0$、$n=0$ 时）。

$\mathit{A}(m,n)=\mathit{A}(m-1,\mathit{A}(m,n-1))$；（$m,n>0$ 时）。

输入m和n，调用akm函数，输出计算结果，并统计函数执行了多少步。

### 函数接口定义：
```python
def akm(m,n):
    pass
```
定义一个函数akm，计算akm(m,n)的结果

### 裁判测试程序样例：
```python
# 在此处填写函数代码
step=0
m,n=map(int, input().split())
print("Reulst:",akm(m,n))
print("Steps:",step)
```

### 输入样例：
在这里给出一组输入。例如：

```python
3 5
```
### 输出样例：
在这里给出相应的输出。例如：

```python
Reulst: 253
Steps: 42438
```