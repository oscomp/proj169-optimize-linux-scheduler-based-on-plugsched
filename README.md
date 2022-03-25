# proj169-optimize-linux-scheduler-based-on-plugsched

## 项目名称

基于 Plugsched 实现 Linux kernel 调度器优化

## 项目描述

[Plugsched ](https://gitee.com/anolis/plugsched)是 Linux 内核调度器子系统热升级的 SDK，它可以实现在不重启系统、应用的情况下动态替换调度器子系统，毫秒级 downtime 。plugsched 可以对生产环境中的内核调度特性动态的进行增、删、改，以满足不同场景或应用的需求，且支持回滚。

基于 plugsched 实现调度器热升级，即使不修改现有内核代码，也能获得较好的可修改能力，天然支持线上的老内核版本。如果提前在内核调度器代码的关键数据结构中加入 Reserve 字段，可以额外获得修改数据结构的能力，进一步提升表达能力。

本项目帮助同学们深入学习调度器相关知识，在 Anolis 7.9 ANCK 4.19 系统中，利用 plugsched，在不修改内核代码的情况下，针对两个典型的应用场景做优化。应用场景自选，可以是常见的 micro benchmark，也可以是真实的应用软件。评价标准如下：

1. 应用软件的使用场景越广泛越好，且真实应用优于 benchmark；
1. 性能提升比列越大越好；
1. 如果能够改进 plugsched 的一些设计缺陷，可以加分；

## 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道

## 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的学生（本科生/研究生均可）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2022国大学生操作系统比赛”的章程和技术方案要求

## 项目导师

陈善佩 :  shanpeic@linux.alibaba.com
吴一昊 :  wuyihao@linux.alibaba.com

## 难度

中等

## License

GPLv2 / BSD

## 开发环境

Plugsched 默认支持 Anolis OS 7.9 ANCK，建议基于 ANCK 内核开发，避免不必要的环境问题。详情参考 [https://gitee.com/anolis/plugsched#quick-start](https://gitee.com/anolis/plugsched#quick-start)

## 预期目标

1. 学习 Linux 内核调度器相关知识和调试方法，掌握调度器子系统热升级的基本原理；
1. 学以致用，针对实际的场景，提升应用的性能；
1. 如果有好的想法，可以为 plugsched 贡献代码；

## 参考资料

[https://gitee.com/anolis/plugsched](https://gitee.com/anolis/plugsched)

