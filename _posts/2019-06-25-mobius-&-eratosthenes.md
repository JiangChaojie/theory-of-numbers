---
title: mobius 函数 μ(n)、Eratosthenes 筛法
---

## 例子

1. 求不超过 100 且与 2，3，5 均互素的正整数的个数。
2. 求不超过 100 的素数个数 $\pi(100)$ 。（利用 `eratosthenes` 筛法）

## 背景知识

1. $M \ddot o bius$ 函数 $\mu(n)$ 定义在 N 上，
   $$
   \mu(n)=
   \begin{cases}
   1, n=1, \\
   (-1)^r, n=p_1\cdots p_r,p_1 \neq\cdots \neq p_r \\
   0, other
   \end{cases}
   $$
   可以推出 $\mu(n)$ 是积性函数，但不是完全积性的。

2. 设 n 是正整数，得到
   $$
   I(n)=\sum\limits_{d\mid n}\mu(d)=[\frac 1 n]=
   \begin{cases}
   1,n=1, \\
   0,n>1.
   \end{cases}
   $$
   证明：首先证明 $I(n)$ 是积性的，得到 $I(1)=1$ ，然后知道 $I(p^\alpha)=1+\mu(p)=0,\alpha\ge 1$

   利用这个式子我们可以提出一个一般方法：对给定的有限整数序列 A 及整数 K，如何去求序列 A 中所有与 K 既约的整数个数。

3. 设 A 是一个给定的有限整数序列，K 是给定的正整数，再设 $A_d$ 表示 A 中被正整数 d 整除的所有整数组成的子序列，$p_1,\cdots,p_s$ 是 K 的所有的不同的素因数，以及 $\mid A_d \mid$ 表序列 $A_d$ 中的整数个数。那么序列 A 中所有与 K既约的数的个数

   $S(A;K)=\sum \limits_{\alpha\in A,(a,k)=1}1=\sum\limits_{d \mid K}\mu(d)\mid A_d\mid$

4. `eratosthenes` 筛法
   $$
   \pi(x)=\pi(\sqrt x)-1 + \sum\limits_{d \mid P(\sqrt x)}\mu(d)[\frac x d] \\
   = \pi(\sqrt x)-1+x \prod\limits_{p\le \sqrt x}(1- \frac 1 p)-\sum \limits_{d \mid P(\sqrt x)} \mu(d)\{\frac x d\}
   $$



{{site.math}}