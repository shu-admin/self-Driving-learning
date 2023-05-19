#### 学习要求
1. 无人驾驶汽车的分类
自动驾驶分级标准

2. 自动驾驶对感知的要求
自动驾驶中需要正确识别的目标
3. 如何做出驾驶决策

#### 自动驾驶术语
1. Driving task(驾驶任务)
- perceiving the environment(环境感知)
> 感知我们驾驶的时候周围的环境 这涵盖了追踪车辆的移动和 识别周围环境中的不同元素 比如路面 交通标志 车辆和行人等 我们还需要追踪所有移动的物体.并预测它们接下来的行动 这样我们才能安全而准确地驾驶 

- Planning how to reach from point A to B(规划)
> 运动规划 这让我们能成功地到达目的地 比如说 你想从你的家驾驶到你的办公室 你需要考虑你会经过哪些路 什么时候应该变道或通过路口 怎么转弯绕过地上的坑

- Controlling the vehicle(控制车辆)
> 最后 我们需要用车辆控制来操作车辆 我们需要做出正确的转向 刹车和加速决定 来控制车辆在路上的位置和速度

这三个子任务构成了 驾驶任务的主体. 它们需要在驾驶过程中被不断地执行

2. operational design domain(ODD)
ODD指明了给定的系统 可以在什么样的操作环境下工作 它包括了环境 时间段 路面条件和其它驾驶过程所需要依赖的因素 在设计环节清晰地定义自动驾驶车辆的操作条件 是确保系统安全性所必需的 所以ODD需要预先仔细设计

3. Lateral control(侧向控制)
转向和巡航。左转 右转 直行或沿着弯道行驶等等

4. Longitudinal Control(纵向控制)
控制车辆在道路上的位置和速度的任务，通过采用刹车和加速之类的动作。

5. Object and Event Detection and Response(OEDR)
OEDR物体和事件检测响应。OEDR检测对驾驶任务有即时影响的 物体和事件 并正确地对它们做出反应 OEDR包含了自动驾驶的很大一部分 所以它和ODD一起 被用来分类现在的自动驾驶系统

6. Planning(规划)

- Long term(长期规划)

> 到达目的地

- Short term(短期规划)
> 变道、通过路口


#### 自动驾驶分级
国际汽车工程师学会在2014年建议的分解（方案）the SAE Standard J3016[https://www.sae.org/standards/content/j3016_201806/.]
1. Level 0 - No Automation
* Regular vehicles, no automation
完全没有自动驾驶涉及 驾驶员完成所有任务

2. Level 1 - Driving Assistance
自动驾驶系统能协助驾驶员 完成侧向控制和纵向控制中的其中一个.
* examples
    - Adaptive Cruise Control
    自适应巡航控制(ACC)系统，系统可以控制车辆的速度，驾驶员来控制方向。它可以完成纵向控制，但需要人来完成侧向控制
    - Lane Keeping Assistance
    车道保持辅助系统，系统可以帮助保持在你的车道上 并在你滑向边界（车道线）的时候给出警告 今天的系统依赖于对车道线的视觉检测 和保持在车道正中的侧向控制

3. Level 2 - Partial Driving Automation
系统在特定场景下同时完成侧向控制和纵向控制。
* examples
  - GM Super Cruise
  - Nissan Propilot Assist
它们可以控制你在侧向和正向上的运动 但驾驶员对系统的监视是始终需要的

4. Level 3 - Conditional Driving Automation
除了控制任务之外 系统还可以在一定程度上进行 物体和事件检测响应 然而 在（系统）故障时 驾驶员必须接管 2级和3级的关键区别在于 （在3级中）驾驶员在某些场景下不需要关注（驾驶过程） 因为车辆会在需要介入时警示司机.

5. Level 4 - High Driving Automation
高度自动驾驶 系统可以做出使危险最小的决策 从而让驾驶员不用在紧急情况下介入 4级系统可以自行处理紧急事件 但仍有可能 需要驾驶员介入来避免不必要的路边停靠

6. Level 5 - High Driving Automation
系统是完全自动化的 设计适用域不再有限制 这意味着它可以在任何必须的条件下运行 5级自动驾驶是我们的社会经历变革的节点 无人驾驶的车辆可以在任何我们需要的时候运输乘客和货物 我们还没有5级自动驾驶的例子