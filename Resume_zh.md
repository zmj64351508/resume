# 周明君

* Email: <nxpzmj@126.com>
* 手机: 13636570382

## 专业技能

* 熟悉Linux内核和驱动
* 熟悉ARM架构

| 语言       | 程度   |  主要使用领域  |
| -------------  | -------------  | -------------  |
| C          | 熟悉    |   Linux kernel/driver, bootloader |
| Python     | 熟悉  |   工具脚本和简单UI   |
| C++        | 能读写  |  浏览/修改Android Framework  |
| Java       | 能读写   | 浏览/修改Android Framework和APP |

## 工作经历

### Senior Software Engineer, OPPO

2017年4月 至今

主要负责内核优化和部分新功能驱动

#### ELSA

- 一套基于cgorup实现了的用于后台冻结的机制

- 内核模块实现:

  - 加速PID和UID的相互转换

  - 在被冻结任务收到重要消息时通知用户空间

  - 通过对齐异步消息减少解冻次数

#### BinderMonitor

* 监控重要服务的binder使用情况

* 内核实现：

  * 在Android binder驱动中增加插桩

  * 计算binder传输的消耗的时间

  * 在binder传输消耗过多时间时向用户空间报告系统信息

  * 监控binder service的所有binder thread使用情况

  * 对重要服务向外发送的binder增加了timeout机制

#### IOBoost

* 通过提高前台IO的优先级实现加速效果

* 内核实现：

  * 实现一个新的io cgroup，并提供`boost`参数指定当前group是否需要加速

  * 在io elevator中加入代码优先取出属于boost group的request

  * 通过io throttle框架实现下发request时对非boost group进行限制

  * 使用ebpf实现了io性能的监控工具

#### 低功耗协处理器驱动

* 设计低功耗协处理的软件架构，包括固件、驱动、HAL、Service
* 设计并实现AP与协处理的通信协议
* 实现协处理内核驱动

### Senior Software Engineer, 上海兆芯集成电路有限公司
2014年7月 - 2017年4月

主要负责驱动、bootloder开发

#### bootloader

- 负责BootROM代码开发和重构，实现secureboot、fastboot协议、eMMC驱动等功能。
- 负责u-boot中的eMMC驱动、配置、启动速度优化等。

####  Linux内核驱动

- IR发送驱动，通过GPIO模拟
- IR接收驱动开发
- eMMC/SD驱动集成和调试

#### FPGA验证

- 两代芯片的FPGA bring up
- eMMC/SD的FPGA验证
- FPGA BootROM开发

#### 工具开发

- 上述开发中使用的一些工具开发，如boot镜像签名工具、秘钥管理工具等

## 教育背景
### 电子与通信工程, 硕士
2012年9月 - 2014年7月  东华大学, 上海

### 通信工程, 本科
2008年9月 - 2012年7月  东华大学, 上海