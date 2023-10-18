# 使用指引

## 如何开机

电源开关短按显示电量，长按开机或关机，并确认电源指示灯亮起，开机后将小车放在附带组装好后的调车台上，打开车体左侧电调开关（电调是电机和舵机中间的控制器，拨动开关会听到电调发出‘嘀 嘀嘀’的声音确定电调启动）

::: tip 说明
注意: 缓慢推动摇杆，多试几次找找感觉，以防撞车。
:::

## 设备关机

::: danger 警告
切勿使用直接关闭总电源的方式给Jetson Nano断电，正确方式是ssh登录Jetson Nano平台，使用命令`sudo shutdown now`关闭系统，当Nano电源指示灯熄灭时，再长按关闭
:::

## 如何充电

在电量显示不足或听到电量报警情况下，我们需要给动力电池充电，充电时是不需要卸下电池的，充电器和电池连接方式如下（具体充电器以实物为准）：

![充电器](https://tianbot-pic.oss-cn-beijing.aliyuncs.com/tianbot/202112211514679.jpg)

## 动力开关功能
#### 电调开关

电调是电机的驱动器，电调自身带有开关，如果电量充足情况下，无法控制电机，我们可以查看一下是否开关正常开始，在车体一侧，我们可以看到如图所示的一个小开关，这个就是电调的使能开关，打开始将听到车体发出滴滴的响声，表示电调已开启。

电调（动力开关），查看是否为Li电模式，F/R模式，开关已开

![电调开关](https://tianbot-pic.oss-cn-beijing.aliyuncs.com/tianbot/202112211514092.jpg)

::: danger 警告
> 注意： 在不使用小车时，为了避免由于电调待机的电力损耗导致动力电池过度放电(过放)造成动力电池报废(不可逆转)的情况，一定要关闭电调开关！
:::



## 无线遥控

TIANRACER使用遥控器DT7进行控制 ，DT7是一款工作于 2.4GHz 频段的无线电通讯设备，该遥控器仅能与DR16接收机搭配使用，该遥控器在开阔室外的最大控制范围可达1000m，内置锂电池，最长工作时间可达到12个小时。

![DT7](https://tianbot-pic.oss-cn-beijing.aliyuncs.com/tianbot/202112211514356.jpg)

向右拨电源开关，开启遥控器。向左拨电源开关，关闭遥控器。
遥控器开启时有提示音，开启后电源指示灯绿灯长亮并伴随蜂鸣器提示音。
左手摇杆前进后退，右手摇杆转向，S1模式控制设置

遥控正常连接可控（使用DJ dt7进行前后、转向控制）
在运动过程中，观察转速变化的线性度，舵机转向的灵敏程度。以确定PID参数是否合适

::: danger 警告
切勿大幅度推动遥控摇杆，会使得车速过快撞击其他物体，极易造成车体损坏。
:::