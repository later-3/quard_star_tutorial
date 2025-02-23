[![Linux ci](https://img.shields.io/github/workflow/status/qqxiaoming/quard_star_tutorial/linux?style=flat-square&logo=linux)](https://github.com/QQxiaoming/quard_star_tutorial/actions/workflows/linux.yml)
[![Windows ci](https://img.shields.io/github/workflow/status/qqxiaoming/quard_star_tutorial/windows?style=flat-square&logo=windows)](https://github.com/QQxiaoming/quard_star_tutorial/actions/workflows/windows.yml)
[![Macos ci](https://img.shields.io/github/workflow/status/qqxiaoming/quard_star_tutorial/macos?style=flat-square&logo=apple)](https://github.com/QQxiaoming/quard_star_tutorial/actions/workflows/macos.yml)
[![Documentation Status](https://readthedocs.org/projects/quard-star-tutorial/badge/?version=latest)](https://quard-star-tutorial.readthedocs.io/zh_CN/latest/?badge=latest)
[![CodeFactor](https://www.codefactor.io/repository/github/qqxiaoming/quard_star_tutorial/badge)](https://www.codefactor.io/repository/github/qqxiaoming/quard_star_tutorial)
[![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/QQxiaoming/quard_star_tutorial.svg)](https://github.com/QQxiaoming/quard_star_tutorial/releases)
[![GitHub All Releases](https://img.shields.io/github/downloads/QQxiaoming/quard_star_tutorial/total.svg)](https://github.com/QQxiaoming/quard_star_tutorial/releases)
[![GitHub stars](https://img.shields.io/github/stars/QQxiaoming/quard_star_tutorial.svg)](https://github.com/QQxiaoming/quard_star_tutorial)
[![GitHub forks](https://img.shields.io/github/forks/QQxiaoming/quard_star_tutorial.svg)](https://github.com/QQxiaoming/quard_star_tutorial)
[![Gitee stars](https://gitee.com/QQxiaoming/quard_star_tutorial/badge/star.svg?theme=dark)](https://gitee.com/QQxiaoming/quard_star_tutorial)
[![Gitee forks](https://gitee.com/QQxiaoming/quard_star_tutorial/badge/fork.svg?theme=dark)](https://gitee.com/QQxiaoming/quard_star_tutorial)

# 基于qemu从0开始构建嵌入式linux系统

[English](./README.md) | 简体中文

![logo](./tutorial/img/img6.gif)

## 引言

本项目旨在真正从0开始构建嵌入式linux系统，为了剖析芯片从上电开始执行第一条指令到整个系统运行，相关应用服务启动，因此不使用市面上真实的板子，基于qemu定制模拟器开发板，且不使用qemu提供的快速加载elf的文件方式，因而我们需要下载qemu源码，自己编写(或使用qemu自带的)硬件ip相关模拟代码定制属于自己的硬件板卡。本项目同步制作[博客专栏](https://blog.csdn.net/weixin_39871788/category_11180842.html)(2021.8.11:目前开始使用readthedocs构建[文档](https://quard-star-tutorial.readthedocs.io/zh_CN/latest/index.html)，与博客内容相同)，因此项目尽量保证每增加一个feature就提交一次，方便索引跟踪开发过程以方便对应到博客的具体章节。

## 环境搭建

ubuntu20.04需要使用apt安装的包:

```shell
sudo apt install ninja-build pkg-config libglib2.0-dev libpixman-1-dev libgtk-3-dev libcap-ng-dev libattr1-dev libsdl2-dev device-tree-compiler bison flex gperf intltool mtd-utils libpulse-dev libalsa-ocaml-dev libsdl2-dev
```

## 硬件架构

下图为目前的虚拟硬件架构，随着项目推进会持续更新。

![硬件架构](./tutorial/img/img3.png)

## 软件流程

下图为目前的软件流程，随着项目推进会持续更新。

![软件流程](./tutorial/img/img4.png)

## 内存分布

下图为目前的内存分布，随着项目推进会持续更新。

![内存分布](./tutorial/img/img5.png)

## 开发记录

[开发日记](./DEVELOPNOTE.md)
