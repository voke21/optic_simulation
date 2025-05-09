# 平面波和球面波复振幅仿真
- 二维＋三维
- 二维：光强分布，相位分布
- 三维：振幅分布，相位分布
## 平面波
定义：在任意时刻、与波矢量相垂直的平面上振幅和位相为常数的光波称为平面波。
波矢量（Wave Vector）通常用符号 k 表示，是一个矢量，用来描述波的传播方向和波长。它的方向与波的传播方向一致。
平面波传播到空间某点的复振幅的一般表达式为：
\begin{aligned}&U(x,y,z)=a\exp(j\mathbf{k}\cdot\mathbf{r})\\&=a\exp[jk(x\cos\alpha+y\cos\beta+z\cos\gamma)]\end{aligned}
### 两点光源干涉
- 类似杨氏双缝干涉，两点光源在自由空间直接相干
- 给出干涉条纹分布
- 注释掉了光强分布曲线

---

## 数值仿真
- 基于惠更斯菲涅尔原理的衍射公式进行仿真
- u2 = u1与h乘积的离散求和

## 本征方程
- 仍是惠更斯菲涅尔原理的衍射公式
- 利用了np.linalg.eig求本征值和本征方程
- 可得到不同模式的像面图
