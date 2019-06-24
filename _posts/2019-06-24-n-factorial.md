---
title: n! 的素因数分解式
---

## 例子

1. 求 $20!$ 的标准素因数分解式。

   不超过 20 的素数有 2，3，5，7，11，13，17，19，根据背景知识 3 得

   $\alpha(2,20)=[20/2]+[20/4]+[20/8]+[20/16] = 10+5+2+1=18$

   然后分别求其他的 $\alpha$ ，然后利用背景知识 4，得到答案，当然考试不需要最终结果。

2. $20!$ 的十进位表示中结尾有多少个零？

   看展开式中乘了多少个 10 即可。也就是求 $10^k \parallel 20!$ 中的 k。

3. 设整数 $a_j>0,(1\le j \le s),n=a_1+a_2+\cdots + a_s$ ，证明；

   $n!/(a_1!a_2!\cdots a_s!)$

   tips: 只需证明 $\alpha(p,n)\ge \alpha(p,\alpha_1) + \alpha(p,\alpha_2)+\cdots +  \alpha(p,\alpha_s)$

   显然 $[n/p^j] \ge [a_1/p^j] + [a_2/p^j]+ \cdots +[a_s/p^j]$

4. 证明 m 个相邻整数的乘积可被 $m!$ 整除。 

## 背景知识

利用符号 $[x]$ 给出 n!  的标准素因数分解式的公式。

1. $n!=p_1^{\alpha_1}\cdots p_s^{\alpha_s}$

2. $a^k\parallel b$ ：b 恰被 a 的 k 次方整除，即

   $a^k \mid b, a^{k+1} \nmid b$

3. 设 n 是正整数，p 是素数，再设 $\alpha=\alpha(p,n)$ 满足 $p^\alpha \parallel n!$ ，那么
   $$
   \alpha = \alpha(p,n)=\sum \limits_{j=1}^{\infty} [\frac{n}{p^j}]
   $$
   右边其实就是一个有限和，因为有上限。

4. 设 n 是正整数，我们有
   $$
   n!=\prod \limits_{p \le n} p^{\alpha(p,n)}
   $$
   



{{site.math}}