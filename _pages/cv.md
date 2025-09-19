---
layout: archive
title: "个人简历"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## 教育经历
* 2022.9-2026.6 北京邮电大学 | 电信工程及管理 | 本科
  * 主修课程：模拟电路、信号与系统、数字电路设计、微处理器系统设计、数字信号处理、通信原理、电磁场与电磁波、互联网协议与网络、高级网络编程
  * 选修课程：C语言、数据结构、JAVA、Python、VHDL技术、人工智能导论、深度学习、Linux系统、模拟CMOS集成电路设计、数字集成电路设计
  * GPA：87/100

## 项目经历
* 2025.3-至今 中国科学院自动化研究所 | 科研实习生
  * 侯增广教授-李国涛教授指导
  * 呼吸采集系统设计：主导设计并实现基于单片机的呼吸信号采集系统，采用嵌入式开发技术优化系统性能，确保高精度、低延迟的生理信号采集与处理
  * 节点预测网络架构设计：负责开发用于预测呼吸关键节点的人工智能Transformer网络架构，结合嵌入式系统实现高效数据处理与实时反馈

* 2024.10-2025.5 CMOS近似加法器设计 | 科研实习生
  * 核心成果：以第一作者在2025 IEEE ICSECE发表论文"ADual-ModePrecision Configurable: Error-CorrectableAdder forEnergy-EficientApplications"，获EI Compendex等数据库收录
  * 技术突破：创新双模式可配置精度架构，实现动态容错与能耗优化，提升神经网络加速器能效

* 2023.9-2024.9 智能语音与情感交互实验室 | 科研实习
  * 李雅教授指导
  * 垃圾分类低开销框架：以第二作者发表"ALow-overheadFrameworkforTrash ClassificationBasedonDenseNet"被ICCEA2025接收，并由IEEE CSCPS出版，收录于EI Compendex、CNKI及Scopus数据库
  * "康慧培优"便民医疗陪护系统：提供AI技术支持，主导智能陪护模块开发与医疗数据可视化，优化用户体验。项目获"互联网+"校级二等奖及国家级大创结项
  * 反电信网络诈骗AI Agent平台：参与智能代理系统开发，构建反诈骗模型并优化训练流程，显著提升平台识别率。团队荣获华为杯全国三等奖

## 实习经历
* 2025.1-2025.7 北京志凌海纳科技股份有限公司(SmartX) | 硬件兼容性测试实习工程师
  * 负责在服务器部署SMTXOS系统、配置网络及部署集群，运用Linux操作系统，结合VMware，开展虚拟化分布式系统领域测试及超融合硬件兼容与一体化产品测试，支撑公司IT基础设施产品线，保障硬件适配性

## 技能专长
* 核心技术栈：Python/C++/VHDL编程开发，STM32CubeIDE/Keil MDK嵌入式开发，Cadence Virtuoso硬件设计，使用Linux系统
* AI开发体系：PyTorch深度学习框架，ONNX/TensorRT模型优化
* 工程实施能力：STM32/CST Design平台开发，MATLAB仿真验证
* 研发协作支撑：Git版本控制全流程，跨团队项目管理与敏捷协作

## 荣誉奖项
* 大学生创新创业训练计划，国家级评审(2024)
* 第六届中国研究生人工智能创新大赛(华为杯)，国家三等奖(2024)
* 中国大学生"互联网+"创新创业大赛，北京邮电大学赛区二等奖(2023)
* 第二届"英语世界"杯全国大学生翻译大赛，全国三等奖(2022)
* 大学英语四级、大学英语六级

## 论文发表
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
## 学术报告
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
## 教学经历
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
## 服务与领导力
* 积极参与开源项目开发和社区贡献
* 在多个科研项目中担任核心开发角色
* 具备良好的团队协作和沟通能力
