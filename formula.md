\[\begin{align}
   {{u}_{H}} =u+q{{z}_{H}}-r{{y}_{H}}  \\
   {{v}_{H}} =v-p{{z}_{H}}+r{{x}_{H}}  \\
   {{w}_{H}} =w+p{{y}_{H}}-q{{x}_{H}}  \\
\end{align}\]


when $\omega =0$
\[\begin{align}
   \dot{u}_{H} =\dot{u}+qw-rv  \\
   \dot{v}_{H} =\dot{v}-pw+ru  \\
   \dot{w}_{H} =\dot{w}+pv-qu  \\
\end{align}\]

\[\begin{align}
\dot{u}_{H} =\dot{u}+qw-rv  \dot{q} z_H-\dot{r} y_H+p q y_H+p r z_H+q^2 \left(-x_H\right)-r^2 x_H \\
\dot{v}_{H} =\dot{v}-pw+ru -\dot{p} z_H+\dot{r} x_H+p^2 \left(-y_H\right)+p q x_H+q r z_H-r^2 y_H \\
\dot{w}_{H} =\dot{w}+pv-qu  \dot{p} y_H-\dot{q} x_H+p^2 \left(-z_H\right)+p r x_H-q^2 z_H+q r y_H \\
\end{align}\]

提取公因式后结果为：
\[\begin{align}
\dot{u}_{H} =\dot{u}+qw-rv + z_H (\dot{q}+p r)+y_H (p q-\dot{r})+x_H \left(-q^2-r^2\right) \\ 
\dot{v}_{H} =\dot{v}-pw+ru + z_H (q r-\dot{p})+x_H (\dot{r}+p q)+y_H \left(-p^2-r^2\right) \\
\dot{w}_{H} =\dot{w}+pv-qu + y_H (\dot{p}+q r)+x_H (p r-\dot{q})+z_H \left(-p^2-q^2\right) \\
\end{align}\]

机体线速度和线加速度转换到旋翼固定坐标系为
\[\begin{bmatrix}
    u_s\\
    v_s\\
    w_s\\
\end{bmatrix}=
\mathbf{T}_{SB}
\begin{bmatrix}
    u_H\\
    v_H\\
    w_H\\
\end{bmatrix}\]

\[\begin{bmatrix}
    \dot{u}_s\\
    \dot{v}_s\\
    \dot{w}_s\\
\end{bmatrix}=
\mathbf{T}_{SB}
\begin{bmatrix}
    \dot{u}_H\\
    \dot{v}_H\\
    \dot{w}_H\\
\end{bmatrix}\]

机体角速度和角加速度转换到旋翼固定坐标系为

\[\begin{bmatrix}
    p_s\\
    q_s\\
    r_s\\
\end{bmatrix}=
\mathbf{T}_{SB}
\begin{bmatrix}
    p\\
    q\\
    r\\
\end{bmatrix}\]

\[\begin{bmatrix}
    \dot{p}_s\\
    \dot{q}_s\\
    \dot{r}_s\\
\end{bmatrix}=
\mathbf{T}_{SB}
\begin{bmatrix}
    \dot{p}\\
    \dot{q}\\
    \dot{r}\\
\end{bmatrix}\]


假设桨叶上任意一点到桨毂中心处的相对位置矢量 $\boldsymbol{r}_p$为
\[r_p=ej_R+rj_{BS}=
x_p i_s+
y_p j_s+
z_p k_s\]


普通的变量x:`x`:$x$
粗体1：使用`\boldsymbol{}`进行加粗，如：`\boldsymbol{x}`:$\boldsymbol{x}$
粗体2：使用`\mathbf{}`进行加粗，如：`\mathbf{x}`:$\mathbf{x}$
带箭头的向量：使用`\vec{}`使向量带箭头，如`\vec{x}`:\vec{x} 作者：科皮子菊 https://www.bilibili.com/read/cv3599113/ 出处：bilibili

式中： e 为桨叶挥舞铰偏置量， r 为桨叶上任意一点到桨叶根部的距离。相对位置矢量 $r_p$的 各分量为

\[\begin{bmatrix}
    x_p\\
    y_p\\
    z_p\\
\end{bmatrix}=
\begin{bmatrix}
    -e\cos\psi-r\cos\beta\cos(\psi+\zeta)\\
    e\sin\psi+r\cos\beta\sin(\psi+\zeta)\\
    -r\sin\beta
\end{bmatrix}\]


桨叶微段转速 U_TU_RU_P
\[
\begin{align\cdot }
u_{T} 
&=-e \left(r_s-\Omega_R\right) \cos \left(\zeta _i\right)\\
&+{y_{2}} p_s \sin \left(\beta _i\right) \cos \left(\zeta _i+\psi \right)-{y_{2}} q_s \sin \left(\beta _i\right) \sin \left(\zeta _i+\psi \right)-{y_{2}} \left(r_s-\Omega_R\right) \cos \left(\beta _i\right)\\
&+u_s \sin \left(\zeta _i+\psi \right)+v_s \cos \left(\zeta _i+\psi \right)\\
u_{R} 
&=-e p_s \sin (\psi ) \sin \left(\beta _i\right)-e q_s \cos (\psi ) \sin \left(\beta _i\right)-e \left(r_s-\Omega_R\right) \cos \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&-u_s \cos (\psi ) \cos \left(\beta _i\right) \cos \left(\zeta _i\right)+u_s \sin (\psi ) \cos \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&+v_s \sin (\psi ) \cos \left(\beta _i\right) \cos \left(\zeta _i\right)+v_s \cos (\psi ) \cos \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&-w_s \sin \left(\beta _i\right)\\
u_{P} 
&=p_s \left(e \sin (\psi ) \cos \left(\beta _i\right)+{y_{2}} \sin \left(\zeta _i+\psi \right)\right)\\
&+q_s \left(e \cos (\psi ) \cos \left(\beta _i\right)-{y_{2}} \sin (\psi ) \sin \left(\zeta _i\right)+{y_{2}} \cos (\psi ) \cos \left(\zeta _i\right)\right)\\
&-e \left(r_s-\Omega_R\right) \sin \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&+u_s \sin (\psi ) \sin \left(\beta _i\right) \sin \left(\zeta _i\right)-u_s \cos (\psi ) \sin \left(\beta _i\right) \cos \left(\zeta _i\right)\\
&+v_s \sin (\psi ) \sin \left(\beta _i\right) \cos \left(\zeta _i\right)+v_s \cos (\psi ) \sin \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&+w_s \cos \left(\beta _i\right)\\
\end{align\cdot }
\]


\[u_{T}=-e\left(r_s-\Omega_R\right)\cos\left(\zeta_i\right)+{y_{2}}p_s\sin\left(\beta_i\right)\cos\left(\zeta_i+\psi\right)-{y_{2}}q_s\sin\left(\beta_i\right)\sin\left(\zeta_i+\psi\right)-{y_{2}}\left(r_s-\Omega_R\right)\cos\left(\beta_i\right)+u_s\sin\left(\zeta_i+\psi\right)+v_s\cos\left(\zeta_i+\psi\right)\]

\[u_{R}=-ep_s\sin(\psi)\sin\left(\beta_i\right)-eq_s\cos(\psi)\sin\left(\beta_i\right)-e\left(r_s-\Omega_R\right)\cos\left(\beta_i\right)\sin\left(\zeta_i\right)-u_s\cos(\psi)\cos\left(\beta_i\right)\cos\left(\zeta_i\right)+u_s\sin(\psi)\cos\left(\beta_i\right)\sin\left(\zeta_i\right)+v_s\sin(\psi)\cos\left(\beta_i\right)\cos\left(\zeta_i\right)+v_s\cos(\psi)\cos\left(\beta_i\right)\sin\left(\zeta_i\right)-w_s\sin\left(\beta_i\right)\]

\[u_{P}=p_s\left(e\sin(\psi)\cos\left(\beta_i\right)+{y_{2}}\sin\left(\zeta_i+\psi\right)\right)+q_s\left(e\cos(\psi)\cos\left(\beta_i\right)-{y_{2}}\sin(\psi)\sin\left(\zeta_i\right)+{y_{2}}\cos(\psi)\cos\left(\zeta_i\right)\right)-e\left(r_s-\Omega_R\right)\sin\left(\beta_i\right)\sin\left(\zeta_i\right)+u_s\sin(\psi)\sin\left(\beta_i\right)\sin\left(\zeta_i\right)-u_s\cos(\psi)\sin\left(\beta_i\right)\cos\left(\zeta_i\right)+v_s\sin(\psi)\sin\left(\beta_i\right)\cos\left(\zeta_i\right)+v_s\cos(\psi)\sin\left(\beta_i\right)\sin\left(\zeta_i\right)+w_s\cos\left(\beta_i\right)\]



相对气流速度 $V_{WP}$ 的幅值 $U_Y$ 和偏斜角 $\gamma_Y$ 分别为

\[
U_Y = \sqrt{
    U_T^2+
    U_R^2+
    U_P^2
    }    
\]

\[
    \gamma_Y = \arccos \frac{|U_T|}{\sqrt{U_T^2+U_R^2}}
\]

旋翼桨叶安装角 $\theta_G$ 可以表示为

\[
    \theta_G =
    \theta_0 
    -\theta_{1C}\cos(\psi+\Delta_{SP})
    -\theta_{1S}\sin(\psi+\Delta_{SP})
    +\theta_{TW}
\]

$\Delta_{SP}$ 为旋翼自动倾斜器提前操纵角， $\theta_{TW}$为旋翼桨叶负扭角，
可以表示为桨叶径向位置的函数

\[
    \theta_{TW}=f(\epsilon+\bar{y}_2)
\]

由桨叶安装角和桨叶相对来流速度各分量，可得桨叶的叶素迎角为

\[
    \alpha_Y = \arctan \left[
        \frac{(U_T \tan\theta_G+U_P)\cos\gamma_Y}{U_T-U_P\tan\theta_G\cos^2\gamma_Y}
    \right]
\]


上面给出的桨叶迎角公式推导过程

在$U_R=0$的情况下，桨叶来流与安装角共同决定的桨叶迎角

\[
    \tan\alpha_Y = \tan\left[\theta_G+\alpha_W\right] \\
    =\frac{\tan\theta_G+\tan\alpha_W}{1-\tan\theta_G\tan\alpha_W}\\
    =\frac{\tan\theta_G+\frac{U_P}{U_T}}{1-\tan\theta_G\frac{U_P}{U_T}}
\]

其中 $\theta_G$ 为桨叶微段安装角， $\alpha_W$为$U_R=0$ 时的来流$U_T,U_P$间的夹角
$\tan\alpha_W = \frac{U_P}{U_T}$

当$U_R$不等于0时，认为整个桨叶微段受到相同的侧向来流
此时 $\tan\theta_G$ 变成 $\tan\theta_G\cdot\cos\gamma_Y$,
而 $\tan\alpha_W$ 变成 $\tan\alpha_W\cdot\cos\gamma_Y = \frac{U_P}{U_T}\cos\gamma_Y$.

\[
    \tan\alpha_Y = \tan\left[\theta_G+\alpha_W\right] \\
    =\frac{\left(\tan\theta_G+\tan\alpha_W\right)\cdot\cos\gamma_Y}{1-\tan\theta_G\cdot\cos\gamma_Y\cdot\tan\alpha_W\cdot\cos\gamma_Y}\\
    =\frac{\left(\tan\theta_G+\frac{U_P}{U_T}\right)\cdot\cos\gamma_Y}{1-\tan\theta_G\frac{U_P}{U_T}\cdot\left(\cos\gamma_Y\right)^2}\\
    =\frac{\left(U_T\tan\theta_G+U_P\right)\cdot\cos\gamma_Y}{U_T-\tan\theta_G U_P\cdot\left(\cos\gamma_Y\right)^2}\\
\]



=======
带偏斜量的气流作用在近似为二元翼型的桨叶微段上得到一组气动力系数 $C_L,C_D$ 一般称之为二元翼型的升力系数和阻力系数。二元翼型假设整个翼型的气动力作用在位于1/4弦线处的气动中心，阻力系数$C_D$的方向与来流方向一致，升力系数$C_L$方向与$C_D$垂直。

二元翼型气动力根据风洞试验得到的数据通过分段线性插值的方法得到。

\[C_D = f\left(\alpha_Y,Mach\right)\]
\[C_L = f\left(\alpha_Y,Mach\right)\]

利用力的归一化因子计算得到桨叶微段上的气动力
$F_{NBS} = \frac{1}{2}\rho\left(\omega R\right)^2 \cdot S_Y$ 

式中 $S_Y$ 为桨叶微段面积， $\rho$ 为当地空气密度， $\Omega R$ 为旋翼桨尖速度。

CLCD可以在桨叶微段的来流坐标系中写作$\left(-C_D,0,C_L\right)$

从桨叶坐标系到桨叶微段来流坐标系经过两次转轴
1. 绕Z轴转过角度 $+\gamma_Y$, 其中 $\tan\gamma_Y = U_R/U_T$
2. 再绕Y轴转过角度 $+\alpha_W$, 其中 $\tan\alpha_W = U_P/\sqrt{U_T^2+U_R^2}$

% todo
上面的转动思路不对 !

% 应该为
% % 1. 绕Y轴转过角度 $+\alpha_W$, 其中 $\tan\alpha_W = U_P/U_T$
% % 2. 绕Z轴转过角度 $+\gamma_Y$, 其中 $\tan\gamma_Y = U_R/U_T$

% 1. 绕Z轴转过角度 $+\gamma_Y$, 其中 $\tan\gamma_Y = U_R/U_T$
% 2. 再绕Y轴转过角度 $+\alpha_W$, 其中 $\tan\alpha_W = U_P/U_T$


我用坐标转换的方法没能成功处理CDCL的坐标转换，因为偏斜角 $\gamma_Y$ 的处理方式是直接乘在两个tan函数上的，



新的思路是将UTUPUR想象成一个长方体，CD方向正好在斜对角线方向上
因此CD的三个分量为

\[F_{TD} = F_{NBS} \cdot  U_Y^2 \cdot  C_D \cdot  U_T/U_Y\]
\[F_{RD} = F_{NBS} \cdot  U_Y^2 \cdot  C_D \cdot  U_R/U_Y\]
\[F_{PD} = F_{NBS} \cdot  U_Y^2 \cdot  C_D \cdot  U_P/U_Y\]

CD方向为 $\left(-U_T,U_R,-U_P\right)$
CDCL所在平面的法向量方向为 $\left(U_R,U_T,0\right)$
二者叉乘得到CL方向的矢量 $\left(U_TU_P,-U_RU_P, -U_T^2-U_R^2\right)$
转换到$U_T,U_R,U_P$方向为$\left(-U_TU_P,-U_RU_P, U_T^2+U_R^2\right)$ xz方向加负号

CL垂直于CD方向，处理时需要通过偏斜角来考虑

\[F_{TL} = F_{NBS} \cdot  C_L \cdot  -U_TU_P
F_{RL} = F_{NBS} \cdot  C_L \cdot  -U_RU_P
F_{PL} = F_{NBS} \cdot  C_D \cdot  (U_T^2+U_R^2)\]

而吉师兄的论文和kim的论文中给出的拉力系数公式部分为
\[F_{TL} = F_{NBS} \cdot  C_L \cdot  -U_PU_Y\cdot \cos\gamma_Y
F_{RL} = F_{NBS} \cdot  C_L \cdot  -U_RU_PU_Y\cdot \cos\gamma_Y/U_T
F_{PL} = F_{NBS} \cdot  C_D \cdot  U_YU_T/\cos\gamma_Y\]

FTFR 这样处理的原因我没弄清楚

=========
由桨叶各叶素的气动力可得单片桨叶根部受到的气动力为
\[
    F_T = \sum_{j=1}^{Ns}F_{Tj}
    F_R = \sum_{j=1}^{Ns}F_{Rj}
    F_P = \sum_{j=1}^{Ns}F_{Pj}
\]

相对挥舞摆振铰的气动力矩为
\[
    M_{\beta}=\sum_{j=1}^{Ns}\left(\bar{y}_{2j} R F_{Pj}\right)
    M_{\zeta}=\sum_{j=1}^{Ns}\left(\bar{y}_{2j} R F_{Tj}\right)
\]

式中： $N_s$ 为单片桨叶上的分段数。

最后，将单片桨叶气动力和气动力矩从桨叶坐标系转换到旋翼旋转坐标系

\[
    \begin{bmatrix}
        F_{XA}\\
        F_{YA}\\
        F_{ZA}\\
    \end{bmatrix}
    =\mathbf{T}_{RBS}
    \begin{bmatrix}
        -F_T\\
        F_R\\
        -F_P\\
    \end{bmatrix}
\]

其中 $\mathbf{T}_{RBS}$ 为 $\mathbf{T}_{BSR}$ 的逆矩阵，由于坐标转换矩阵为正交矩阵，使用转置方法就可以计算坐标转换阵的逆矩阵。

========

桨叶动力学方程

桨叶任意一点运动速度为

\[
    V_P = V_H + \omega\times r_p
\]

对时间求导得到 桨叶任意一点加速度

\[
    a_p = a_H + \dot\omega\times r_p + \omega\times\left(
        \omega\times r_p + \frac{\partial r_p}{\partial t}
    \right)
\]


由桨叶运动加速度得到单位长度桨叶惯性力和惯性力矩分别为

\[dF = \rho_b a_p dr\]
\[dM = r\times dF\]

$\rho_b$为桨叶单位长度质量，
$r$为桨叶微段到桨叶根部的相对位置矢量？？
桨叶根部还是挥舞摆振铰处？ 从后文看应该是挥舞摆振铰处

由上式积分得到作用于挥舞摆振铰处的惯性力就分别为
\[ M_{\beta I} =  L_I =  \int_e^R -r \rho a_{ZPBS} dr \]
\[ M_{\zeta I} = -N_I = -\int_e^R -r \rho a_{XPBS} dr = \int_e^R r\rho a_{XPBS} dr \]

式中 $\rho$ 为空气密度，$a_{XPBS},a_{YPBS},a_{ZPBS}$ 为桨叶上任意一点加速度 $a_p$ 在桨叶坐标系中的分量，且

\[
    \begin{bmatrix}
        a_{XPBS}\\
        a_{YPBS}\\
        a_{ZPBS}\\
    \end{bmatrix}
    =\mathbf{R}_{BSR}
    \begin{bmatrix}
        a_{XP}\\
        a_{YP}\\
        a_{ZP}\\
    \end{bmatrix}
\]


铰链处的气动力矩、惯性力矩、弹簧约束力矩和摆振阻尼器产生的力矩平衡关系如下所示：
\[
    M_{\beta A}+
    M_{\beta I}+
    M_{\beta K}+
    M_{\beta LD}=0
\]

\[
    M_{\zeta A}+
    M_{\zeta I}+
    M_{\zeta K}+
    M_{\zeta LD}=0
\]

$M_{\beta K},  M_{\zeta K}$ 为挥舞、摆振方向的弹簧约束力矩
$M_{\beta LD},  M_{\zeta LD}$ 为挥舞、摆振方向由摆振阻尼器产生的力矩

根据力矩平衡方程计算处的挥舞运动和摆振运动方程为：


? 弹簧力矩呢
\[I_{b} \ddots{\beta_i} = M_{\beta LD} + M_{\beta A} + M_{\beta I}\]

