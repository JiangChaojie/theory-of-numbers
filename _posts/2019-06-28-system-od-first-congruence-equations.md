---
title: 一次同余方程组、孙子定理
---

## 实例

1. 解同余方程组
   $$
   \begin{cases}
   x\equiv1(mod \ 3), \\
   x\equiv -1(mod \ 5), \\
   x \equiv 2 (mod \ 7), \\
   x \equiv -2(mod \ 11)
   \end{cases}
   $$

2. 求相邻的四个整数，它们依次可被 $2^2,3^2,5^2$ 及 $7^2$ 整除。

3. 求模 11 的一组完全剩余系，使其中每个数被 $2,3,5,7$ 除后的余数分别为 $1,-1,1,-1$ 。

4. 解同余方程组

   $x\equiv3(mod \ 8),x\equiv11(mod \ 20),x\equiv 1(mod \ 15)$

5. 解同余方程 $19x\equiv 556(mod \ 1155)$

6. 解同余方程组

   $x\equiv3(mod \ 7),6x\equiv10(mod \ 8)$

7. 解同余方程组

   $3x\equiv1(mod \ 10),4x\equiv7(mod \ 15)$

## 背景知识

本节讨论一次同余方程组。

1. 孙子定理

   设 $m_1,\cdots,m_k$ 是两两既约的正整数，那么，对任意整数 $a_1,\cdots,a_k$ ，一次同余方程组

   $x\equiv a_j(mod \ m_j),1\le j \le k \cdots(1)$

   必有解，且解数为 1，事实上，同余方程组（1）的解是

   $x\equiv M_1M_1^{-1}a_1 + \cdots + M_kM_k^{-1}a_k(mod \ m)\cdots(2)$

   这里 $m=m_1\cdots m_k,m=m_jM_j(1\le j \le k)$ ， 以及 $M_j^{-1}$ 是满足

   $M_jM_j^{-1}\equiv 1(mod \ m_j),1\le j\le k$

   的一个整数（即是 $M_k$ 对模 $m_j$ 的逆）。

2. $x\equiv M_1M_1^{-1}x_1 + \cdots + M_kM_k^{-1}x_k\cdots(3)$

   当 $x_1,\cdots,x_k$ 分别遍历模 $m_1,\cdots$ ，模 $m_k$ 的完全（既约）剩余系时，x 遍历模 m 的完全（既约）剩余系时，x 遍历模 m 的完全（既约）剩余系，且有

   $x\equiv x_j(mod \ m_j),1\le j \le k$

3. 设 $a_1,\cdots,a_k$ 是给定整数，$(a_j,m_j)=1,1\le j\le k$ ，再设

   $x^*=M_1a_1x_1+\cdots+M_ka_kx_k\cdots(4)$

   那么当 $x_1,\cdots, x_k$ 分别遍历模 $m_1,\cdots$ ，模 $m_k$ 的完全（既约）剩余系时，$x^*$ 遍历模 m 的完全（既约）剩余系。

4. Euler 函数 φ(m) 时积性函数，即

   $\phi(m_1,m_2)=\phi(m_1)\phi(m_2),(m_1,m_2)=1.$

5. 设 $m_1,\cdots,m_k$ 两两互素，$m=m_1\cdots m_k$ ，以及 $f(x)$ 是整系数多项式，我们有

   $T(f;m)=T(f;m_1)\cdots T(f;m_k)$

   这里 $T(fn)$ 表示同余方程 $f(x)\equiv0(mod \ n)$ 的解数，也就是说，解数 $T(f;n)$ 是 n 的积性函数。

{{site.math}}