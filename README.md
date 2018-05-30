CARLA Simulator
===============
CARLA is an open-source simulator for autonomous driving research. CARLA has
been developed from the ground up to support development, training, and
validation of autonomous urban driving systems. In addition to open-source code
and protocols, CARLA provides open digital assets (urban layouts, buildings,
vehicles) that were created for this purpose and can be used freely. The
simulation platform supports flexible specification of sensor suites and
environmental conditions.

ToDo
-------
- [ ] Play around with CarLa simulator in Unreal.
- [ ] Potentially add a Radar sensor.
- [ ] Test with NVIDIA Model for behavorial cloning project.
- [ ] Add mouse control for steering wheel.(It works better comparing to AWSD). 

Random Thoughts
-------
一些Simulation Design的想法。
首先，为什么需要simulation.因为数据的收集一部分可以是来自显示生活，另一部分是可以来自虚拟环境。
使虚拟环境趋于显示，不仅仅意味着画面的渲染使现实风格，更重要的是模拟现实环境的各种参数，提供的各种信息，比如说，在进行lane line finding的时候，会被环境中的很多类似早晚光照，地面不平，天气情况，的很多因素影响，这个环境因素是有可能在虚拟环境中被模拟出来的。
* different levels based on weather, light condition, and etc

第二个原因，当我们设计无人车的时候，会考虑到各种传感器，通过设计不同的传感器module, 应用于不同场景进行测试，这个针对不同企业的需求，可customized的传感器suit可以被设计出来。

第三个原因，2017年加州新增了30个无人驾驶测试的拍照，很多无人驾驶公司都在进行的收集数据的活动，现实生活中的路面状况非常复杂，但是也会出现开了很多miles, 都没有出现的极端情况。我们可以使用模拟器，收集极端交通事故的信息，模拟这个极端案例，从而预防一些corner case的产生。
第四个原因，随着人工智能的发展，我认为可以模拟器的运行可以是automated, 意思是可以交由算法来穷尽各种运算，用人工智慧来模拟各种情况
