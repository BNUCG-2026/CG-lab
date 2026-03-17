# 🚀 万有引力粒子群仿真

> 本项目为图形学课程实验环境配置与基础实践，主要内容包括：

现代 Python 开发环境（uv）配置

Taichi 高性能计算库安装

图形学项目结构（src layout）规范

GPU 粒子系统仿真实现（万有引力粒子群）

---

# 📌 Introduction


This project focuses on **data preprocessing and analysis for station-based traffic datasets**.

It provides tools to automatically convert raw `.xlsx` data into structured `.npy` datasets and supports visualization and statistical analysis.

该项目主要实现了粒子群跟随鼠标

---

# 🎬 Demo

实验结果展示：

![实验演示视频](https://github.com/Wu-Zhongxia/CG-lab/blob/main/video/N4UWoUKr_converted.gif)

---

# 📂 Project Structure

```
CG_Lab/
├── pyproject.toml         <-- uv 自动生成的项目配置文件
├── src/
│   └── Work0/             <-- 实验零专属包
│       ├── __init__.py    <-- 空文件，标识这是一个 Python 包
│       ├── config.py      <-- 存放所有可调参数
│       ├── physics.py     <-- 存放 GPU 并行计算与物理逻辑
│       └── main.py        <-- 程序的入口文件，负责 GUI 渲染
```

---

# ⚙ Installation

## Environment

推荐环境：

```
Python = 3.12
```

## Install dependencies

```bash
pip install -r requirements.txt
```

如果没有 requirements 文件：

```bash
pip install numpy pandas matplotlib seaborn
```

---

# 🚀 Usage

## 1 Data preprocessing

将数据文件放入目录：

```
data/
```

运行：

```bash
python scripts/all_pre.py
```

---

## 2 Run analysis

```bash
python main.py
```

输出结果：

```
results/
figures/
```
---

# 🧪 Experiments

实验内容包括：

### Dataset

| Dataset | Description |
| --- | --- |
| Station Data | Traffic data for multiple stations |
| Processed Data | Cleaned dataset for analysis |

### Evaluation

实验指标：

- 数据处理效率
- 算法运行时间
- 结果准确性

---

# ⚙ Configuration

配置文件示例：

```
config.yaml
```

示例：

```yaml
data_path: ./data
output_path: ./results
visualization: true
```

---

# 👨‍💻 Authors

```
Shirley Wu
School of Artificial Intelligence
Beijing Normal University
```
