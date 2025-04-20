元素: $\alpha$ $\beta$ $x$ $y$
向量: $\vec{x_i} = \left[x_1^i, x_2^i \ldots x_3^i,x_m^i \right]$
    $\vec{\beta} = \left[\beta_0, \beta_1 \ldots \beta_2,\beta_m \right]$

$$y_i \approx \beta_0 + \sum_{j=1}^n  \beta_j \times x_j^j$$

向量xi扩展:$\vec{x_i} \approx \left[1, x_1^i, x_2^i \ldots x_3^i,x_m^i \right]$

$$y_i \approx \sum_{j=0}^m  \beta_j \times x_j^j=\vec{\beta} \cdot \vec{x}$$

$$\hat{\vec{\beta}} = \arg\min_{\vec{\beta}} L(D, \vec{\beta}) = \arg\min_{\vec{\beta}} \sum_{i=1}^{n} (\vec{\beta} \cdot \vec{x}_{i} - y_{i})^{2}$$

矩阵：$\mathbf{X}$ $\mathbf{Y}$ 
转置：$mathbf{X}^\top$

$$L(D, \vec{\beta}) 
= \|\mathbf{X}\vec{\beta} - \mathbf{Y}\|^2= (\mathbf{X}\vec{\beta} - \mathbf{Y})^\top (\mathbf{X}\vec{\beta} - \mathbf{Y})= \mathbf{Y}^\top\mathbf{Y} - \mathbf{Y}^\top \mathbf{X}\vec{\beta} - \vec{\beta}^\top \mathbf{X}^\top \mathbf{Y} + \vec{\beta}^\top \mathbf{X}^\top \mathbf{X}\vec{\beta}$$

分数: $\frac {X} {Y}$
偏导 $\partial L $ $\partial \beta$ 

$$\frac{\partial L(D,\vec\beta)} {\partial\vec\beta} = \frac{\partial L}{\partial \vec{\beta}} = - 2\mathbf{X}^\top\mathbf{Y}+2\mathbf{X}^\top\mathbf{X}\vec{\beta}$$

梯度设置为0:
$$-2\mathbf{X}^\top\mathbf{Y}+2\mathbf{X}^\top\mathbf{X}\vec{\beta} = 0\Rightarrow \mathbf{X}^\top\mathbf{X}\vec{\beta} = \mathbf{X}^\top\mathbf{Y}\Rightarrow \vec{\beta} = (\mathbf{X}^\top\mathbf{X})^{-1}\mathbf{X}^\top\mathbf{Y}$$

