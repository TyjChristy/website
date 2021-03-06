+++
title = "开发"
description = ""
weight = 3
+++

# 开发

## 1. 概述

开发是项目的重要步骤，本章节将围绕和开发相关的各个功能的使用进行详细的介绍，包括应用服务、迭代计划、代码管理，将涵盖您在开发过程中所有可在平台中进行的操作。

## 2. 应用服务

应用服务是指Choerodon平台中能提供某项具体服务的最小单元。一般地，一个应用可由多个应用服务组成，其中，每个应用服务仅关注完成一部分任务，而每部分任务又代表了一个小的业务模块，因此各个应用服务之间的关系是松耦合的。

此外，在Choerodon平台的项目层中每创建或导入一个应用服务时，GitLab上都会生成一个与之对应的代码仓库。

了解如何创建和导入应用服务，详情请查看[应用服务](./application-service)。

## 3. 代码管理

代码管理包含了与开发过程相关的一系列操作及流程，其中包括 [分支管理](./code-manage/manage-branch)、[合并请求](./code-manage/merge-request)、[持续集成](./code-manage/integration)、[标记](./code-manage/sign)以及[代码质量](./code-manage/code-quality)

了解如何用Choerodon代码管理模块进行开发，详情请查看[代码管理](./code-manage)
