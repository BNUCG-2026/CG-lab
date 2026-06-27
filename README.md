# 计算机图形学实验1 - 万有引力粒子群仿真

202411081009 吴仲霞 计算机科学与技术

## 一、实验目的

本实验旨在完成图形学开发环境的搭建，并通过一个简单的粒子系统程序，掌握以下内容：

* Python 项目环境配置（uv）
* Taichi 并行计算库的使用
* 基本图形学程序结构设计
* GPU 粒子仿真实现

## 二、实验环境

* 操作系统：Windows11
* CPU：AMD R7
* GPU：NVIDIA RTX 4060
* 开发工具：TRAE IDE
* Python版本：3.12
* 包管理工具：uv
* 核心依赖：taichi

## 三、项目结构

```
CG-Lab/
├── pyproject.toml        # 项目配置文件（uv 管理依赖）
├── README.md             # 项目说明文档  
├── uv.lock               
├── .gitignore               
├── .python-version               
├── video                 # 存放演示视频
    └── N4UWoUKr_converted.gif
│
└── src/
    └── Work0/
        ├── __init__.py
        ├── config.py     # 参数配置
        ├── physics.py    # GPU并行计算
        └── main.py       # 程序入口 + GUI渲染
```

## 四、环境配置步骤

### 1. 安装 IDE

下载并安装 TRAE：
[https://www.trae.cn/ide/download](https://www.trae.cn/ide/download)

### 2. 安装 uv

#### Windows11：

```bash
pip install uv
```

验证安装：

```bash
uv --version
```

### 3. 初始化项目

```bash
uv init --python 3.12
uv sync
```

### 4. 安装依赖

```bash
uv add taichi
```

## 五、实验内容说明

本实验实现了一个**基于万有引力的粒子系统仿真**，主要功能如下：

* 初始化大量粒子（默认 10000 个）
* 鼠标位置作为引力源
* 粒子受到引力、阻力影响运动
* 碰到边界后发生反弹

## 六、核心模块说明

### 1. config.py

用于统一管理参数，例如：

* 粒子数量
* 引力强度
* 窗口大小
* 粒子颜色

### 2. physics.py

负责底层物理计算：

* 使用 Taichi GPU 并行计算
* 更新粒子位置和速度
* 处理边界碰撞

### 3. main.py

程序入口，负责：

* 初始化 Taichi
* 获取鼠标位置
* 渲染粒子动画

## 七、运行方式

在项目根目录下执行：

```bash
uv run -m src.Work0.main
```

运行后会弹出窗口：

* 移动鼠标 → 粒子被吸引
* 粒子会在窗口内反弹运动

## 八、实验结果演示

实验结果展示：

![实验演示视频](https://github.com/Wu-Zhongxia/CG-lab/blob/main/video/N4UWoUKr_converted.gif)
