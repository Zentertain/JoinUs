Zentertain Developer Interview Quiz
===================================

TODO basic requirement
* Object Oriented Design
* Clean Code
* Unit Test / Test?
* Git history

背景
----------

> NASA 正在计划一个叫做MarsRover的新计划。这个计划是一轮新的火星探索，科学家将投放一组无人驾驶的火星探测车 MarsRover 到火星表面，做地面探索。

> MarsRover 计划有一组研究课题组成，你可以从中选择一个你有兴趣的参加

## 1. Compass 项目

> Compass 项目 主要是做火星路线的规划。火星表面有一组需要观测的兴趣地点(PoI)，NASA希望Mars Rover可以以某种顺序探索其中的特定的一部分。

Quiz 1:

规划后的路由使用有向图来描述，其中节点表示的是PoI，边表达的是PoI之间的路径，边的权重表示的是MarsRover从其中一个点移动到另外一个点所消耗的能量。边的起点和终点不会为同一个。

从探索有效性的角度出发，所有的路径都是单行的，有从A到B的路径不代表有从B到A的路径。事实上，如果正向、反向的路径确实同时存在的话，它们将是不同的两条路径，并且权重不一定相同。

### Input:

AB5 BC4 CD8 DC8 DE6 AD5 CE2 EB3 AE7
A->E
A->D->E

### Expected Output:
The shortest route from A to E
The shortest route from A To E passes D
