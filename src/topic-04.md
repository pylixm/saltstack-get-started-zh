# SaltStack 组件

您将在本教程中获得对这些组件的更好的测试介绍，但对于每个组件在SaltStack中的作用的一般概念来说，下面这些内容是有帮助的。

## Salt Master 

中央管理系统。该系统用于向托管系统上运行的Salt minion发送命令和配置。

<img src="/saltstack/./src/./media/salt-master.png" width = "150" height = "200" alt="图片名称" align=center />

## Salt Minions

管理系统。该系统运行Salt Minion，它从Salt主机接收命令和配置。

<img src="/saltstack/./src/./media/salt-minions.png" width = "150" height = "200" alt="图片名称" align=center />

## 执行 module 

从命令行针对一个或多个受管系统执行的临时命令。作用：
- 实时监控，状态和清单。
- 一次性命令和脚本的运行。
- 部署关键的更新。

<img src="./saltstack/./src/./media/execution-modules.png" width = "200" height = "200" alt="图片名称" align=center />

## Formulas (States)

系统配置的声明或命令式表示。

<img src="/saltstack/./src/./media/formulas.png" width = "200" height = "200" alt="图片名称" align=center />

## Grains

系统变量。grains 是关于底层管理系统的静态信息，包括操作系统，内存和许多其他系统属性。您还可以为任何系统自定义grains。

<img src="/saltstack/./src/./media/grains.png" width = "200" height = "200" alt="图片名称" align=center />

## Pillar

用户相关定义的变量。这些安全变量被定义并存储在Salt Master上，然后使用`targets` “分配”到一个或多个分区。`pillar`存储了端口，文件路径，配置参数和密码等值。

<img src="/saltstack/./src/./media/pillar.png" width = "200" height = "200" alt="图片名称" align=center />

## Top File 

使`Formulas`和 `salt pillars`数据与 `minion`对应起来。

<img src="/saltstack/./src/./media/top-file.png" width = "200" height = "200" alt="图片名称" align=center />

## Runners

在Salt Master上执行的任务模块。`Salt Runner`可以报告任务状态，连接状态，从外部API读取数据，查询连接的`Salt Minion`等。

<img src="/saltstack/./src/./media/runners.png" width = "350" height = "300" alt="图片名称" align=center />

## Returners

将`Salt minions`返回的数据发送到另一个系统，如数据库。`Salt Returners`可以在`Minion`或`Master`上运行。

<img src="/saltstack/./src/./media/returners.png" width = "350" height = "300" alt="图片名称" align=center />

## Reactor

当您的SaltStack环境发生事件时触发反应。(译者注：类似事件总线上的监听函数，特定时间出发)

<img src="/saltstack/./src/./media/reactor.png" width = "350" height = "300" alt="图片名称" align=center />

## Salt Cloud 

为云提供商/管理程序提供系统，并立即将其管理。

<img src="/saltstack/./src/./media/salt-cloud.png" width = "600" height = "300" alt="图片名称" align=center />

## Salt SSH 

在没有`minion` 的机器上通过SSH的方式运行命令。

<img src="/saltstack/./src/./media/salt-ssh.png" width = "150" height = "200" alt="图片名称" align=center />




