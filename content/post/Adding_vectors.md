+++
date = '2025-03-21T16:02:15+08:00'
draft = true
title = 'Adding vectors'
tags = ['Math']
tags_weight = 20

+++

# 向量的加减，直线参数方程的推导

{{< katex >}}

> Adding vectors

$\vec{a}=\begin{bmatrix} 2\newline2\end{bmatrix}$ 和 $\vec{b}=\begin{bmatrix} 3\newline-3\end{bmatrix}$

把两个向量加到一起我们会得到：

$$
\vec{a}+\vec{b}=\begin{bmatrix}2+3\newline2-3 \end{bmatrix}=\begin{bmatrix}5\newline-1 \end{bmatrix}
$$
![a+b](/ill/addab.png)

你会发现实际上就是把 \\(vec{b}\\) 平移到 \\(vec{a}\\) 的终点。你可以这么理解，向量的 \\(vec{a}+vec{b}\\) 其实就是先从 0 点走到 \\(a\\) 点，然后在走到与 \\(\vec{b}\\) 相等的量到达 \\(\vec{a}+\vec{b}\\) 点。

减法会怎样？
$$
\vec{b}-\vec{a}=\begin{bmatrix}3-2\newline-3-2 \end{bmatrix}=\begin{bmatrix}1\newline-5 \end{bmatrix}
$$

![b-a](/ill/b-a.png)

可以看出把 \\(\vec{b}-\vec{a}\\) 平移到 \\(\vec{a}\\) 的终点，就是从 \\(a\\) 点出发到 \\(b\\) 点，也就说，\\(\vec{b}-\vec{a}\\) 可以理解成从 \\(a\\) 点 出发到 \\(b\\) 点的距离。

到这里如果我们给 \\(\vec{b}-\vec{a}\\) 乘以一个标量(Scalar)，你会发现这就是一个经过起点 \\(a\\) 经过 \\(b\\) 点的一条直线，而参数方程 \\(L=\{\vec{a}+t(\vec{a}-\vec{b}|t\in\mathbb{R})\}\\) 就是一个关于a 和 b的直线集合，标量的大小可以随意缩放这条直线。

举个例子，这里我们假设 \\(t=2.5\\)
$$
设t=2.5\newline L=\begin{Bmatrix}2+2.5(3-2)\newline2+2.5(-3-2)\end{Bmatrix}=\begin{bmatrix}4.5\newline-10\end{bmatrix}
$$
我们可以得到 \\(x = 4.5, y = -10\\)，这就是把 \\(\vec{b}-\vec{a}\\) 放大了2.5倍得到的一个向量。假设 \\(t=1\\) 的话那么我们正好可以得到一个 \\(\vec{b}-\vec{a}\\) 的向量。如果 \\(t<0\\)，那么线就是往反方向走了。

把图画出来：

<img src="/ill/SetL.png" alt="SetL" style="zoom: 80%;" />

红线就是参数方程表达的直线，我们只需要控制 \\(t\\) 的大小就可以得到这个直线上的任意一个点（向量）。