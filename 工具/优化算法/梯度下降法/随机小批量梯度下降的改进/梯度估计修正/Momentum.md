动量法（Momentum Method）是用之前积累动量来替代真正的梯度． 每次迭代的梯度可以看作加速度．
惯性保持, 惯性体现在对前一次步伐信息的重利用上
参数的迭代公式:`v(t)=γv(t-1)+ηg(t)
θ(t+1)=θ(t)+v(t)`, 其中v(t)：当前前进步伐, g(t)：当前估计梯度, η：学习率, γ：衰减系数

算法名的由来
动量（Momentum）是模拟物理中的概念． 一个物体的动量指的是该物体在它运动方向上保持运动的趋势， 是该物体的质量和速度的乘积． 类比中学物理: v(t-1)：前一时刻前进步伐: 前一时刻的速度; g(t)：当前估计梯度:当前时刻受力产生的加速度; v(t)：当前前进步伐:考虑前一时刻的速度和当前加速度共同作用;γ：衰减系数:扮演阻力.
“山谷陷阱”,
向下动量不断累积, 向下速度越来越快, 左右动量累积的结果是相互抵消, shi收敛速度更快, 收敛曲线更稳定