+++
title = "组织层次"
description = ""
weight = 3
+++

### 组织层次
---

Choerodon中有三层组织层次，即全局层、组织层和项目层。Choerodon使用三层组织结构来管理用户、权限、项目、环境资源、菜单，以及其他系统资源和功能。Choerodon这样的设计其实是借用的SaaS组织管理概念，主要是Choerodon应用开发框架为了满足用户SaaS化的需求而设计的，在Choerodon的应用开发和运营管理中使用的不多。

下面我们将从如下几个方面来阐述Choerodon的组织层次：

- [全局层](#全局层)
- [组织层](#组织层)
    - [运营组织](#运营组织)
- [项目层](#项目层)

### 全局层
---
Choerodon的全局层中包含了系统的一些基本设置，例如组织管理、菜单管理、全局角色管理等。另外，在全局层还可以查看Choerodon系统中的服务和权限分配等。

全局层可以包含多个组织，例如运营组织。

### 组织层
---

Choerodon使用组织来管理用户、权限、项目、环境资源，以及其它系统资源和功能。在系统中有一个默认的组织**运营组织**，目前Choerodon中所有的服务、功能和资源都定义在整个组织下面。举个例子，有一个零售公司，想通过Choerodon搭建一个基于微服务的数字化服务平台，此平台涵盖了从门店、零售到库存等整个供应链的管理，需要开发门店管理服务、零售服务、支付服务、库存服务、商品服务等，此时我们可以整个公司看做一个组织，将数字服务平台中包含的所有服务放在这个组织下。当然，如何以项目的形式开发，我们将在项目层中说明。

一个组织可以包含多个项目，例如智能监控。

#### 运营组织

运营组织是Choerodon自带的缺省组织，Choerodon平台上所有的基础服务全部放在次组织下面。例如，用户服务、权限服务、看板服务、Gitlab服务等。

### 项目层
---

Choerodon通过项目来管理软件的开发，项目属于组织，在