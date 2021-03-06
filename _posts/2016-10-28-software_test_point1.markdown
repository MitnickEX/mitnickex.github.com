---
layout:     post
title:      "软件测试知识点总结(1)"
subtitle:   "快速入门上篇"
date:       2016-10-28
author:     "MitnickEX"
header-img: "img/post-bg-software-test-point.jpg"
tags:
    - 软件测试
    - 总结
---

*之前的发的都是一些技术文章，貌似不是特别接地气……趁着公司要来新人，今天带来一点浅显易懂的测试基础……但是基本会想到哪儿写哪儿，所以也许会比较乱……那么，来死狗~*
![](http://i.imgur.com/rQDaWrr.jpg)

[软件测试知识点总结-快速入门上篇](http://mitnickex.github.io/2016/10/28/software_test_point1/)

[软件测试知识点总结-快速入门中篇](http://mitnickex.github.io/2016/10/31/software_test_point2/)

[软件测试知识点总结-快速入门下篇](http://mitnickex.github.io/2016/11/02/software_test_point3/)

首先，软件测试是什么鬼？
> 软件测试：特定的环境、特定的条件下运行软件，验证其能正常运行，并发现其缺陷，对软件的质量进行评估的过程

然后，软件测试有什么鬼流程？
> 软件测试流程：需求、计划、方案、用例、执行、总结

# 1、测试需求 #
#### 测试需求分析：分析识别测试范围，解决测什么的问题，方便测试的跟踪和管理 ####
- **测试需求分析的流程**：需求采集—>需求分析—>需求评审；
- **测试需求分析的评审**：完整性、准确性、一致性、易理解性、无歧义性；
- **测试需求分析的时间**：开发需求完成后；
- **负责人**：有丰富经验的测试工程师；
- **参考依据**：需求规格(狭义)，参照上面的测试需求分析来源(广义)；
- **在测试需求不明确的情况下，如何保证测试质量**：

	（1）多方收集需求；
	
	（2）多与开发人员沟通；
	
	（3）若有以前的系统，参照以前的系统；
	
	（4）找类似的产品熟悉；
	
	（5）到网上查找与系统相关的业务知识、专业术语；

- **测试需求分析的来源**：

	（1）开发文档：需求规格、概设、详设、数据库结构设计文档、模块功能图等；
	
	（2）用户需求：与用户或需求分析人员沟通，需求调研的会议纪要，与用户邮件往来；
	
	（3）软件雏形：可运行软件，软件的框架；
	
	（4）相关的规划及标准：各行各业的标准、国家标准、行业标准、企业标准、项目标准、国家法律法规；
	
	（5）类似的产品：公司内部相同的旧版本产品，行业其他公司类似的产品；
	
	（6）测试知识经验库：测试人员的业务背景、系统业务知识的积累、个人的测试经验积累；
	
	（7）其他隐性的需求：产品利益相关者的建议、会议纪要、备忘录、沟通记录、邮件往来等；

- **测试需求分析的内容**：

	（1）业务流程图的分析；
	
	（2）用户和角色的分析；
	
	（3）数据库结构的分析；
	
	（4）测试要点的分析；

- **测试需求分析的方法**：

	（1）测试功能点分析法；
	
	（2）功能交互分析法；
	
	（3）质量特性分析法；
	
	（4）测试类型分析法；
# 2、测试计划 #

### 测试计划：管理层文档，对测试过程、测试活动起到指导的作用，解决做什么的问题 ###

- **测试计划编写时间**：测试需求完成之后；
- **编写人**：由项目测试负责任编写；
- **评审人**：项目经理、QA、开发、产品、设计人员
- **输出文档**：总的测试计划文档；
- **测试计划的内容**：

	（1）项目背景，缩略语（专业术语）；
	
	（2）测试的参考文档、测试的交付文档；
	
	（3）测试目标、测试范围、测试环境、测试工具、测试策略、测试风险；
	
	（4）人力资源的分配、工作量的估算；
	
	（5）测试时间、进度安排、任务分配、培训计划等；
	
	（6）出入口准则（准入准出标准）等；

|项目|项目时间周期|测试用例数量|
|---|---|---|
|小|	3个月—10个月|500-1000个|
|中|10个月—1.5年|1000-2000个|
|大|	1.5年以上|2000个以上|

- **测试风险**：质量、时间进度、成本、变更、人员变动等；
- **QA与QC的区别**：QA为质量保证、QC为质量控制；
- **冒烟测试**：在测试之前，对软件进行可测性检查，保证基本功能，基本流程可通，提高工作效率；
- **回归测试**：包括完全回归和部分回归（根据操作频率和风险选择）

|测试阶段|	占用时间比例|
|---|---|
|测试需求阶段|	10%-20%|
|测试计划|	小项目2-3天，大项目5天左右|
|测试方案|	小项目1周，大项目2周|
|测试用例|	测试总时间的30%|
|测试执行|	测试总时间的40%|
|测试报告|	小项目2-3天，大项目5天|
 
    编写测试用例效率：35个/人天；
    执行测试用例效率：35个/人天；
    缺陷发现效率：10个/人天；
    测试用例的质量：30%（缺陷的总数/已执行的测试用例总数）

- **集成策略**：

	（1）非增量式集成：大爆炸式集成；
	
	（2）增量式集成：自顶向下、自底向上、三明治；
	
	测试准入条件：
	
	（1）测试用例编写，测试评审完成；
	
	（2）开发人员完成编码，并完成自测；
	
	（3）冒烟测试通过；
	
	（4）开发组提交了测试申请单；

- **测试准出条件**：

	（1）时间标准：项目时间用尽；
	
	（2）缺陷修复：致命/严重缺陷比率为0%，一般<5%，轻微<10%;
	
	（3）测试用例执行覆盖率为100%；
	
	（4）测试用例对需求覆盖率>95%;
	
	（5）缺陷修复率达到一定的标准；
	
	（6）收益比：存在bug，但是修复需要花费的时间大于受益，测试停止；
	
	（7）完成软件测试验收报告，并且报告结果达到认可；

---
**To be continued**