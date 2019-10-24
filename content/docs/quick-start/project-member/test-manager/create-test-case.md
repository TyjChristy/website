+++
title = "创建测试用例"
weight = 1
description = "介绍如何快速创建测试用例"
+++

## 创建一个测试用例
---

## 概述

测试用例功能能够帮助企业管理用例测试的过程，沉淀测试记录和结果，实现随时回溯和量化考核。创建测试用例详细讲解请移步[创建测试用例](../../../../user-guide/test/store/create/)。

## 目标

本页面用于引导用户创建一个测试用例。以创建“`自我介绍模块`”这个测试用例为例。

## 前置条件

**1.** 在操作之前保证[系统配置](../../../../user-guide/manager-guide/system-configuration)已经配置完全。

**2.**用户必须拥有目标项目的`项目成员`或`项目所有者`的权限。

**3.**将测试用例添加到测试循环中需要基于敏捷管理的版本，所以您必须先在敏捷管理中[创建对应的版本](../../../../user-guide/cooperation/work-lists/)。

## 创建一个测试用例

具体操作步骤如下：

**第一步：** 在`测试用例管理`页面点击`创建测试用例`或`创建问题`按钮。

**第二步：** 输入概要(必填)、优先级（必填）、描述（可选）、版本（必填）、文件夹（可选）、经办人（可选）。

例如，

 - 概要：自我介绍模块测试用例
 - 优先级：高
 - 版本：0.10.0

**第三步：** 点击`创建`即可创建一个新的测试用例。

**第四步：** 测试用例创建后，可以在`测试用例管理`页面看到新建的用例。

## 为测试用例添加测试步骤

具体操作步骤如下：

**第一步：** 点击目标测试用例，在测试用例详情页点击`添加测试信息`按钮。

**第二步：** 填写测试步骤（必填）、测试数据、预期结果（必填）。

例如，

 - 测试步骤：自我介绍功能
 - 预期结果：回复预定的自我介绍内容

**第三步：** 点击`创建`即可在用例中添加一个步骤。

**第四步：** 添加完成后，可在用例详情页面的`测试详细信息`栏中看到新添加的测试步骤。并可在表格中直接对内容进行编辑。

![](/img/docs/quick-start/project-member/test-manager/create-test-case/create-test-case-done.png)

## 添加测试用例到测试循环中

具体操作步骤如下：

**第一步：** 点击版本后的`创建文件夹`，以创建一个文件夹

![](/img/docs/quick-start/project-member/test-manager/create-test-case/create-folder.png)

**第二步：** 在目标文件夹内创建一个测试用例。

![](/img/docs/quick-start/project-member/test-manager/create-test-case/create-issue.png)

**第三步：** 在测试计划页面在对应版本的一个循环下添加一个测试阶段，并将测试阶段关联用例所在的文件夹。

![](/img/docs/quick-start/project-member/test-manager/create-test-case/create-stage.png)

**第四步：** 添加阶段后，文件夹内的用例会自动添加相应的执行。

![](/img/docs/quick-start/project-member/test-manager/create-test-case/create-done.png)

## 执行测试

具体操作步骤如下：

**第一步：** 在测试执行页选中对应阶段，在右侧的`测试执行`表格中可以看到上文中添加的测试执行，在测试执行列表里点击对应执行的 ![](/img/docs/user-guide/test-management/case-management/execution-button.jpg) 按钮。

**第二步：** 按照`测试详细信息`栏中的测试步骤进行测试，测试完每一步后，点击表格进行步骤详情记录。

**第三步：** 若测试通过，则将修改状态为通过。若测试失败，则修改状态为失败，并关联缺陷，添加描述。

**第四步：** 测试完所有步骤后，根据测试结果修改`执行状态`，若失败则选择缺陷。

**第五步：** 并且可以在`执行记录中`看到执行的信息变更记录。

![](/img/docs/quick-start/project-member/test-manager/create-test-case/create-show.png)

## 相关文档

- [测试用例管理](../../../../user-guide/test/store/)