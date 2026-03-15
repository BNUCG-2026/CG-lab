# 🚀 Project Name

> A brief description of the project.
> 
> 
> 简要说明该项目解决的问题以及主要功能。
> 

---

# 📖 Table of Contents

---

# 📌 Introduction

介绍项目背景与研究目标。

示例：

This project focuses on **data preprocessing and analysis for station-based traffic datasets**.

It provides tools to automatically convert raw `.xlsx` data into structured `.npy` datasets and supports visualization and statistical analysis.

该项目主要实现：

- 数据预处理
- 批量文件处理
- 数据可视化
- 实验分析

应用场景包括：

- 数据分析
- 科研实验
- 机器学习数据准备

---

# 🎬 Demo

实验结果展示：

![实验演示视频](https://github.com/Wu-Zhongxia/CG-lab/blob/main/video/N4UWoUKr_converted.gif)

# ✨ Features

主要特点：

- ⚡ **High Efficiency** — 自动批量处理数据
- 📊 **Visualization Support** — 数据可视化分析
- 🔄 **Automated Pipeline** — 自动化数据处理流程
- 🧩 **Modular Design** — 代码结构清晰
- 📁 **Multi-file Processing** — 支持批量文件转换

---

# 🏗 System Architecture

系统整体架构：

```
Raw Data (.xlsx)
        │
        ▼
Data Preprocessing
        │
        ▼
Structured Dataset (.npy)
        │
        ▼
Analysis / Modeling
        │
        ▼
Visualization & Results
```

---

# 📂 Project Structure

```
project-name/
│
├── data/                  # 原始数据
├── processed_data/        # 处理后的数据
│
├── scripts/               # 数据处理脚本
│   ├── pre.py
│   └── all_pre.py
│
├── models/                # 模型代码
├── experiments/           # 实验代码
├── figures/               # 可视化结果
├── results/               # 实验结果
│
├── main.py                # 主程序
├── requirements.txt       # 依赖库
└── README.md
```

---

# ⚙ Installation

## Environment

推荐环境：

```
Python >= 3.8
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

程序会自动：

- 扫描所有 `.xlsx` 文件
- 执行数据清洗
- 转换为 `.npy` 文件

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

# 🔄 Workflow

项目运行流程：

```
1. Collect raw data
2. Preprocess data
3. Convert dataset format
4. Run analysis / modeling
5. Visualize results
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
