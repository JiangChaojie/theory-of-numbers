---
title: 数论函数
---

## 例子

1. 设 $n=p_1^{\alpha_1}\cdots p_r^{\alpha_r}$ ，定义在 N 上的数论函数
   $$
   \omega(n)=
   \begin{cases}
   r,n>1; \\
   0,n=1.
   \end{cases}
   $$

   $$
   \Omega(n)=
   \begin{cases}
   \alpha_1 + \cdots + \alpha_r,n>1; \\
   0,n=1
   \end{cases}
   $$

   显见，$w(n)$ 是 n 的不同的素因数的个数，$\Omega(n)$ 是 n 的全部素因数（按重数计）的个数，这两个函数是否为积性？由他们可引入另外两个数论函数

   $\upsilon(n)=(-1)^{\omega(n)},n\ge 1$

   $\lambda(n)=(-1)^{\Omega(n)},n\ge 1$

   $v(n)$ 是积性函数，但不是完全积性的。$\lambda(n)$ 则是完全积性函数它称为 **Liouville 函数**。

2. 设 $d\in Z$ 。证明如下函数是完全积性的
   $$
   h(d)=
   \begin{cases}
   (-1)^{(d-1)/2}, 2\nmid d, \\
   0,2\mid d.
   \end{cases}
   $$
    

## 背景知识

自变量为整数，因变量为复数的数列称为**数论函数**或**算术函数** 。

1. 积性函数

   m,n 属于整数集合 D，且

   $f(mn)=f(m)f(n),(m,n)=1$ 

   则 $f(n)$ 称为时**积性函数** 。
   
2. 完全积性函数

   $f(mn)=f(m)f(n)$ ，但是不要求 $(m,n)=1$

3. 两个（完全）积性函数之积及商（分母恒不为零）都是（完全）积性函数。

4. 设 $f(n)$ 是不恒为零的数论函数，$n=p_1{\alpha^1}\cdots p_r^{\alpha_r}$ 

   $f(n)$ 是积性函数的充要条件是

   $f(1)=1$ 及 $f(n)=f(p_1^{\alpha_1})\cdots f(p_r^{\alpha_r})$

   $f(n)$ 是完全积性的充要条件是 

   $f(1)=1$ 及 $f(n)=f^{\alpha_1}(p_1)\cdots f^{\alpha_r}(p_r)$

   

   



{{site.math}}