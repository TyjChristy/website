+++
title = "快速搜索"
description = "通过定义快速搜索，可以在待办事项和活跃冲刺的快速搜索工具栏生效，帮助您更好的筛选过滤问题面板"
weight = 2
+++

快速搜索可以让用户自定义定制筛选条件，满足了不同用户对于问题的筛选需求。

通过定义快速搜索，可以在待办事项和活跃冲刺的快速搜索工具栏生效，帮助您更好的筛选过滤问题面板。

{{< note >}}
目前的快速搜索只应用在问题（issue）中，且只会在待办事项与活跃冲刺页面中显示。系统会默认初始化两个筛选条件：**仅我的问题**、**仅故事**
{{< /note >}}

## 菜单层级

* 菜单层次：项目层
* 菜单路径：敏捷管理>设置>快速搜索
* 默认角色：项目成员

## 操作步骤

* 创建快速搜索
    1. 点击页面上方的`创建快速搜索`
    2. 在弹出的创建框中输入`名称`（必输）、`筛选条件`（包括`属性`、`关系`、`值`，可支持多个条件共同搜索）、`关系`（若有多个筛选条件，需要添加此关系）、`描述`（可选项）
        ![](/docs/user-guide/agile/setup/img/create-quick-search.jpg)

        目前支持的快速搜索属性有:
        * 经办人
        * 优先级
        * 状态
        * 报告人
        * 创建时间
        * 更新时间
        * 创建人
        * 更新人
        * 故事点
        * 剩余时间
        * 史诗
        * 冲刺
        * 标签
        * 模块
        * 修复的版本
        * 影响的版本
        * 类型
    3. 点击创建即可创建一个新的筛选器
    4. 快速搜索创建成功后，进入到`待办事项`、`活跃冲刺`页面可以看到该筛选器，用户可根据自身需求选择是否应用该快速搜索
        ![](/docs/user-guide/agile/setup/img/result-quick-search.jpg)
* 修改快速搜索
    1. 点击`详情`按钮
    2. 在弹出的修改快速搜索弹窗中，可以对`名称`、`筛选条件`、`关系`及`描述`进行修改
    3. 点击`修改`按钮保存修改
* 删除快速搜索
    1. 点击`删除`按钮
    2. 在弹出的删除框中点击`删除`按钮确认删除
    {{< warning >}}删除后将无法使用该快速搜索{{< /warning >}}