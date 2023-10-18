# Devops Super

## 功能

本项目的定位目标是一个成为一个轻量、易使用、易部署、功能丰富的运维管理平台，**目前还处于开发迭代阶段**，已实现以下功能：

- [x] 基础系统功能：用户管理、部门管理、角色管理、权限管理；
  - [x] 一套权限管理逻辑控制前后端路由、按钮级别权限；
- [x] 堡垒机功能：主机管理、主机组管理；
  - [x] 支持密码、秘钥方式建立 SSH Web 终端（基于 WebSocket）；
  - [x] 支持 Web 文件管理器（上传、下载、删除）管理主机文件系统（基于 WebSocket + SFTP）；
  - [x] 支持终端会话记录持久化到硬盘、回放会话；
  - [x] 支持主机访问授权（主机所属主机组授权到角色或用户）；

开发中：

- [ ] 基于 Kubernetes 原生 Pod 的持续集成（CI）；
  - [x] 秘钥管理；
  - [x] 构建环境管理；
  - [x] 流水线管理（编排）；
  - [x] 运行流水线 & 构建流水线客户端镜像；
  - [x] 流水线运行历史展示；
  - [x] 获取流水线运行日志；
  - [ ] 流水线参数化支持；
  - [ ] 支持挂载指定卷到指定目录；

## 预览地址

[点我预览](http://ds-demo.zze.xyz)

- 管理员：`admin`，密码：`devops.zze`；
- 测试账号：`test`，密码：`devops.zze`；

> 数据库每小时自动重置。

效果图：

![用户管理](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/user-manage.png)
![角色管理](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/role-manage.png)
![权限管理](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/permission-manage.png)
![部门管理](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/dept-manage.png)
![主机管理](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/host-manage.png)
![主机组授权](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/host-group-authorize.png)
![主机终端记录](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/host-terminal-session-history.png)
![全屏终端](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/terminal-single.png)
![终端文件管理器](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/terminal-file-manager.png)
![终端主机树](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/terminal-tree.png)
![流水线管理](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/pipeline-manage.png)
![流水线编排](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/pipeline-arrange.png)
![流水线日志](https://raw.githubusercontent.com/zze326/devops-super/main/resource/imgs/pipeline-log.png)

## 技术栈

- 语言：Golang、Typescript；
- 后端：GoFrame、Casbin；
- 前端：Vue3、Vite、Element-Plus、TypeScript、Pinia 等；

## 项目运行

```
pnpm install
pnpm dev
```

## 后端项目

本仓库是前端项目，对应后端项目地址为：<https://github.com/zze326/devops-super>。
