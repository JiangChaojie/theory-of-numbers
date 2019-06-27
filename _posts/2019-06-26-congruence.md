---
title: 同余
---

## 例子

1. 求 $3^{406}$ 写成十进位数时的个位数。

2. 求 $3^{406}$ 写成十进位数时的最后两位数。

3. 证明：$641\mid 2^{2^5} +1$。

4. 证明不定方程 $x^2+2y^2=203$ 无解。

5. 设 $n\ge 1$ ，b 的素因数都大于 n。证明：对任意正整数 a 必有

   $n!\mid a(a+b)(a+2b)\cdots (a+(n-1)b)$

6. 设 $m>n\ge1$ ，求最小的 m+n 使得

   $1000 \mid 1978^m-1978^n$

## 背景知识

1. 同余

   $a \equiv b(mod \ m)$ ，也就是 a-b=km，**b 是 a 对模 m 的剩余** 。

2. 同余的充要条件是最小非负余数相等。

3. 同余具有自反性，对称性和传递性。因此可以有同余类。

4. 若 $a\equiv b(mod \ m) , c \equiv d(mod \ m)$ 

   1.  $a+c \equiv b+d (mod \ m).$
   2. $ac\equiv bd(mod \ m)$

5. 设 $f(x) =a_nx^n+\cdots+a0,g(x)=b_nx^n+\cdots+b_0$ 是两个整系数多项式，满足

   $a_j\equiv b_j(mod \ m),0\le j \le n \cdots (2)$

   那么，若 $a \equiv b(mod \ m)$ ，则 $f(a)\equiv g(b)(mod \ m)$ 

   我们把满足条件 （2）的两个多项式 $f(x),g(x)$ 称为 多项式 $f(x)$ 同余于多项式 $g(x)$ 模 m。

   注意：函数同模不一定相应系数相同。

6. $a \equiv b(mod \ m),d \mid m$ 则，$a\equiv b(mod \ d)$

7.  $da\equiv db(mod \ \mid d\mid m)$

8. $ca\equiv cb (mod \ m)$

9. 若 $m\ge 1,(a,m)=1$ ，则存在 c 使得

   $ca\equiv 1(mod \ m)$

   我们把 c 称为是 a 对模 m 的**逆** ，记作 $a^{-1}(mod \ m)$ 或 $a^{-1}$ 。

10. 同余式组 $a\equiv b(mod \ m_j),j=1,2,\cdots,k$ 同时成立的充要条件是

    $a\equiv b(mod \ [m_1,\cdots,m_k]).$




{{site.math}}