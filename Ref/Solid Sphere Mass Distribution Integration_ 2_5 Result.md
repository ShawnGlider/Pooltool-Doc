# Solid Sphere Mass Distribution Integration: 2/5 Result

这个 **2/5** 是**用微积分对实心球的质量分布积分**算出来的，是经典刚体力学里的标准结果。我用尽量清晰、一步一步的方式给你推一遍，不用复杂符号也能看懂思路。

# 1\. 转动惯量的定义

转动惯量本质就是：
把物体切成无数小块，每一块的
$dm \cdot r^2$
全部加起来（积分）：
$I=\int r^2 dm$

对**绕球心的旋转轴**，我们要积分整个球体。

# 2\. 球坐标下的积分思路

实心球：

- 半径 $R$

- 密度均匀 $\rho$

- 体积元 $dV = r^2 \sin\theta ,dr d\theta d\phi$

- 质量元 $dm = \rho ,dV$

到转轴的垂直距离不是 $r$，而是
$r_\perp = r\sin\theta$

所以：
$I=\int r_\perp^2 dm = \int (r\sin\theta)^2 \cdot \rho r^2\sin\theta ,dr d\theta d\phi$

$I = \rho \int_0^R r^4 dr \int_0^\pi \sin^3\theta d\theta \int_0^{2\pi} d\phi$

分别积分：

1. $\displaystyle \int_0^R r^4 dr = \frac{R^5}{5}$

2. $\displaystyle \int_0^\pi \sin^3\theta d\theta = \frac{4}{3}$

3. $\displaystyle \int_0^{2\pi} d\phi = 2\pi$

相乘：
$I = \rho \cdot \frac{R^5}{5} \cdot \frac{4}{3} \cdot 2\pi = \rho \cdot \frac{8\pi R^5}{15}$

# 3\. 用总质量 $m$ 替换密度

球质量：
$ m = \\frac\{4\}\{3\}\\pi R^3 \\rho \\quad\\Rightarrow\\quad \\rho = \\frac\{3m\}\{4\\pi R^3\} $

代入 $I$：
$I = \frac{3m}{4\pi R^3} \cdot \frac{8\pi R^5}{15} = \frac{24\pi m R^5}{60\pi R^3} = \frac{2}{5}mR^2$

# 4\. 最终结果

$\boxed{I = \frac{2}{5},mR^2}$

# 5\. 一句话总结

**2/5 就是对实心球做体积分后，化简出来的纯数学系数**，不是经验值，也不是拟合值，是严格几何 \+ 质量分布决定的常数。

---

如果你想，我可以顺便给你推：

- 圆盘 $I=\frac12 mR^2$

- 圆环 $I=mR^2$

- 空心球壳 $I=\frac23 mR^2$

这些系数的来源逻辑完全一样，只是积分区域不同。

> （注：文档部分内容可能由 AI 生成）
