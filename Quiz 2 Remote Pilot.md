Zentertain Developer Interview Quiz
===================================

背景
----------

> NASA 正在计划一个叫做MarsRover的新计划。这个计划是一轮新的火星探索，科学家将投放一组无人驾驶的火星探测车 MarsRover 到火星表面，做地面探索。

> MarsRover 计划有一组研究课题组成，你可以从中选择一个你有兴趣的参加

## 2. Remote Pilot 项目

> Remote Pilot 项目主要是负责开发 MarsRover 的远程巡航控制系统。MarsRover能够接受一系列的指令，并根据指令移动。

MarsRover 接受下列指令:

* M: 前进1个单元
* L: 左转90度
* R: 右转90度
* B: 后退一个单元

假设需要探索的区域是一个方形区域。Rover的位置和朝向使用一组x,y坐标和一个字母表示。'N','S','E','W'分别表示“北”，“南”，“东”，“西”

    0,0,N 表示Rover在坐标 0,0 的位置，并且朝向是北

坐标 0，0位于地图的左下角，如图所示：


	^ N
	|
	|
	|
	|_ _ _ _ _ _>
	0,0         E


如果同时释放多个Rover，那么所有的Rover会同时行动，如果某一回合Rover的目标位置被其他Rover占据，则原地待命一个回合，下一回合再次尝试执行该指令。

如果Rover移动出了探索区域，Rover将并输出DEAD，并且忽略后续指令。

### Input

	20,20 // 探索区域的长宽
	0,0,N
	MMMMRMMMRMMMRLMMMR
	3,3,E
	MMRMRMMRRMRMLM

### Expected Output

	每一个指令周期小车的坐标和朝向

