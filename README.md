# 构思

## 重点突出

1、逻辑组装分发开放

2、数据驱动

## 需要

服务器原子操作库

业务逻辑组装业务

业务逻辑可导入导出数据库存储库

高度可自定义数据模型业务

数据模型数据/动作触发连接编辑

在用户使用层需要加入用户、角色、流程、权限、审计

## 具体代码库

### dashboard(看板)

从中央仓库拉取资源

以套版的方式展示数据(类似grafana),可从分发库拉取数据

通过工作流编排操作并封装

批量单级及多级数据的CRUD会伴随着后端的特殊动作进行而进行

操作数据后拥有进度查询和日志查看

### designer(设计师)

#### 数据

由元数据和数据和数据目录组成

元数据由数据类型和数据骨骼描述组成

模型提供时间版本化以及简易改动分析描述

数据之间可以任意单向连接并直接接入值引用

#### 指令

由原生底层代码编写

#### 业务

由 指令+逻辑+数据 组成

### distribution(分发库)

类似docker的distribution

分为公有仓库和私有仓库

### engine(引擎,加载执行)

#### 加载业务逻辑结合数据执行

#### agent
