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


桨叶微段转速 UTUPUR
\[
\begin{align*}
u_{T} 
&=-e \left(r_s-\Omega_R\right) \cos \left(\zeta _i\right)\\
&+{y_{2}} p_s \sin \left(\beta _i\right) \cos \left(\zeta _i+\psi \right)-{y_{2}} q_s \sin \left(\beta _i\right) \sin \left(\zeta _i+\psi \right)-{y_{2}} \left(r_s-\Omega_R\right) \cos \left(\beta _i\right)\\
&+u_s \sin \left(\zeta _i+\psi \right)+v_s \cos \left(\zeta _i+\psi \right)\\
u_{P} 
&=-e p_s \sin (\psi ) \sin \left(\beta _i\right)-e q_s \cos (\psi ) \sin \left(\beta _i\right)-e \left(r_s-\Omega_R\right) \cos \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&-u_s \cos (\psi ) \cos \left(\beta _i\right) \cos \left(\zeta _i\right)+u_s \sin (\psi ) \cos \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&+v_s \sin (\psi ) \cos \left(\beta _i\right) \cos \left(\zeta _i\right)+v_s \cos (\psi ) \cos \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&-w_s \sin \left(\beta _i\right)\\
u_{R} 
&=p_s \left(e \sin (\psi ) \cos \left(\beta _i\right)+{y_{2}} \sin \left(\zeta _i+\psi \right)\right)\\
&+q_s \left(e \cos (\psi ) \cos \left(\beta _i\right)-{y_{2}} \sin (\psi ) \sin \left(\zeta _i\right)+{y_{2}} \cos (\psi ) \cos \left(\zeta _i\right)\right)\\
&-e \left(r_s-\Omega_R\right) \sin \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&+u_s \sin (\psi ) \sin \left(\beta _i\right) \sin \left(\zeta _i\right)-u_s \cos (\psi ) \sin \left(\beta _i\right) \cos \left(\zeta _i\right)\\
&+v_s \sin (\psi ) \sin \left(\beta _i\right) \cos \left(\zeta _i\right)+v_s \cos (\psi ) \sin \left(\beta _i\right) \sin \left(\zeta _i\right)\\
&+w_s \cos \left(\beta _i\right)\\
\end{align*}
\]


\[u_{T}=-e\left(r_s-\Omega_R\right)\cos\left(\zeta_i\right)+{y_{2}}p_s\sin\left(\beta_i\right)\cos\left(\zeta_i+\psi\right)-{y_{2}}q_s\sin\left(\beta_i\right)\sin\left(\zeta_i+\psi\right)-{y_{2}}\left(r_s-\Omega_R\right)\cos\left(\beta_i\right)+u_s\sin\left(\zeta_i+\psi\right)+v_s\cos\left(\zeta_i+\psi\right)\]

\[u_{P}=-ep_s\sin(\psi)\sin\left(\beta_i\right)-eq_s\cos(\psi)\sin\left(\beta_i\right)-e\left(r_s-\Omega_R\right)\cos\left(\beta_i\right)\sin\left(\zeta_i\right)-u_s\cos(\psi)\cos\left(\beta_i\right)\cos\left(\zeta_i\right)+u_s\sin(\psi)\cos\left(\beta_i\right)\sin\left(\zeta_i\right)+v_s\sin(\psi)\cos\left(\beta_i\right)\cos\left(\zeta_i\right)+v_s\cos(\psi)\cos\left(\beta_i\right)\sin\left(\zeta_i\right)-w_s\sin\left(\beta_i\right)\]

\[u_{R}=p_s\left(e\sin(\psi)\cos\left(\beta_i\right)+{y_{2}}\sin\left(\zeta_i+\psi\right)\right)+q_s\left(e\cos(\psi)\cos\left(\beta_i\right)-{y_{2}}\sin(\psi)\sin\left(\zeta_i\right)+{y_{2}}\cos(\psi)\cos\left(\zeta_i\right)\right)-e\left(r_s-\Omega_R\right)\sin\left(\beta_i\right)\sin\left(\zeta_i\right)+u_s\sin(\psi)\sin\left(\beta_i\right)\sin\left(\zeta_i\right)-u_s\cos(\psi)\sin\left(\beta_i\right)\cos\left(\zeta_i\right)+v_s\sin(\psi)\sin\left(\beta_i\right)\cos\left(\zeta_i\right)+v_s\cos(\psi)\sin\left(\beta_i\right)\sin\left(\zeta_i\right)+w_s\cos\left(\beta_i\right)\]
