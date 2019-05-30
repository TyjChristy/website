﻿+++
title = "客户端"
weight = 4
description = "是对多个客户端信息设置的管理"
+++

# 客户端

客户端是对多个客户端信息设置的管理。配置文件中应用指定的客户端后，登录后跳转页面指向的该客户端设定的网址。

  - **菜单层次**：组织层
  - **菜单路径**：组织设置 > 客户端
  - **默认角色**：组织管理员

<h2 id="1">客户端列表</h2>

列表字段：

- **客户端名称**:客户端名称具有唯一性，是客户端的标识。
- 授权类型：客户端必须得到用户的授权（authorization grant），才能获得令牌（access token），进而凭令牌获取本平台资源。目前平台提供password、implicit、client_credentials、authorization_code和refresh_token五种授权方式。

<h2 id="2">客户端查询</h2>

可查询字段：

- **客户端名称**:客户端名称具有唯一性，是客户端的标识。可根据客户端名称模糊搜索。

<h2 id="3">创建客户端</h2>

1.点击`创建`→![创建](/docs/user-guide/system-configuration/tenant/image/create.png)创建客户端；

2.系统默认生成客户端`名称`和`密钥`。你也可以修改客户端名称和密钥。

3.系统默认授权类型为全选，包括`password`、`implicit`、`client_credentials`、`authorization_code`、`refresh_token`。

4.输入`访问授权超时时间`，默认为3600秒。

5.输入`授权超时时间`，默认为3600秒。

  ![](/docs/user-guide/system-configuration/tenant/image/client.png)

必填字段:

- **客户端名称**:系统默认生成，可修改。客户端名称具有唯一性，是客户端的标识。
- **密钥**：系统默认生成，可修改。使用客户端的密码。例如用户登陆需要用户名和密码，密钥相当于密码。
- 授权类型：系统默认全选。客户端必须得到用户的授权（authorization grant），才能获得令牌（access token），进而凭令牌获取本平台资源。下面提供了五种授权方式：
    1. password：密码模式，用户向客户端提供自己的用户名和密码。客户端使用这些信息，向"服务商提供商"索要授权。
    1. implicit：简化模式，不通过第三方应用程序的服务器，直接在浏览器中向认证服务器申请令牌，跳过了"授权码"这个步骤，因此得名。所有步骤在浏览器中完成，令牌对访问者是可见的，且客户端不需要认证。
    1. client_credentials：客户端模式，客户端以自己的名义，而不是以用户的名义，向"服务提供商"进行认证。严格地说，客户端模式并不属于OAuth框架所要解决的问题。在这种模式中，用户直接向客户端注册，客户端以自己的名义要求"服务提供商"提供服务，其实不存在授权问题。
    1. authorization_code：授权码模式，是功能最完整、流程最严密的授权模式。它的特点就是通过客户端的后台服务器，与"服务提供商"的认证服务器进行互动。
    1. refresh_token：表示早前收到的更新令牌，如果用户访问的时候，客户端的"访问令牌"已经过期，则需要使用"更新令牌"申请一个新的访问令牌。

选填字段：

- 访问授权超时：access_token_validity，assecc token的有效时间。默认为3600秒。
- 授权超时：refresh_token_validity，refresh token的有效时间。默认为3600秒。

3.点击`确定`完成客户端的创建。

<h2 id="4">修改客户端</h2>

1.点击`修改`→![修改](/docs/user-guide/system-configuration/tenant/image/update.png)，对客户端进行修改；

2.修改`密钥`和`授权类型`等可修改信息。

不可修改字段：

- **客户端名称**:客户端名称具有唯一性，是客户端的标识。客户端创建成功后，客户端名称不可更改。

可修改字段：

- 密钥：使用客户端的密码。例如用户登陆需要用户名和密码，密钥相当于密码。
- 授权类型：客户端必须得到用户的授权（authorization grant），才能获得令牌（access token），进而凭令牌获取本平台资源。
- 访问授权超时：access_token_validity，assecc token的有效时间。
- 授权超时：refresh_token_validity，refresh token的有效时间。
- 作用域：作用域为申请的授权范围。最多可输入6个域。
- 自动授权域：自动授权域为oauth认证后，系统自动授权而非用户手动添加的作用域。最多可输入6个域。
- 重定向地址：用户的登陆后从登陆界面跳转的地址。
- 附加信息：用json格式添加客户端的附加信息。如{ "description": "string"，"name": "string"}。

3.点击`确定`完成客户端的修改。

<h2 id="5">删除客户端</h2>

点击`删除图标`→ ![删除按钮](/docs/user-guide/system-configuration/tenant/image/del_button.png)，即可删除客户端。

## 更多操作
- [项目管理](../project)
- [用户管理](../user)
- [LDAP](../ldap)

