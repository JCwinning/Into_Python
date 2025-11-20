# Python 数据科学手册

使用 Quarto 构建的 Python 数据科学学习综合资源。本手册提供实用的示例、分步教程和真实世界的数据分析、可视化和机器学习应用。

## 🌐 在线网站

访问手册：[https://jcwinning.github.io/Into_Python/](https://jcwinning.github.io/Into_Python/)

## 📚 内容概览

本手册涵盖 Python 数据科学所需的一切知识：

### 介绍 (`intro/`)
- **Python 基础**：安装、设置和基本编程概念
- **Python 书籍**：重要的阅读资源和参考资料
- **数据书籍**：数据分析的专业指南
- **统计书籍**：统计概念和应用

### 数据操作 (`data manipulation/`)
- **输入/输出**：读写各种数据格式（CSV、Excel、Parquet 等）
- **数据结构**：理解 Python 内置数据类型和结构
- **Pandas**：全面的数据分析和操作
- **Polar**：Python 高性能数据框
- **SQL 数据库**：处理结构化数据
- **Siuba**：基于语法的数据操作

### 数据可视化 (`plot/`)
- **Seaborn**：统计数据可视化
- **Plotnine**：Python 中的图形语法实现
- **Plotly**：交互式网络可视化

### 发布与分享 (`Publish/`)
- **Shiny**：构建交互式网络应用
- **Quarto**：创建可重现的文档和报告

### 高级主题 (`other/`)
- **网络爬虫**：从网站提取数据（包含真实示例的综合指南）
- **网络爬虫项目**：包括威士忌数据抓取的实用示例

## 🎯 目标受众

本手册适用于：
- **初学者**：刚接触 Python 编程
- **数据分析师**：转向 Python 的分析师
- **数据科学家**：寻找综合参考材料
- **研究人员**：希望学习 Python 数据分析
- **学生**：寻求实践性、动手学习材料

## 🚀 入门指南

### 快速开始
1. **访问在线网站**获得最佳阅读体验
2. **克隆此仓库**以便本地运行代码：
   ```bash
   git clone https://github.com/jcfly3000/Into-Python.git
   cd Into-Python
   ```
3. **安装 Quarto**以便本地渲染文档：
   ```bash
   # macOS
   brew install quarto

   # 或从 https://quarto.org/ 下载
   ```
4. **本地预览网站**：
   ```bash
   quarto preview index.qmd
   ```

### 先决条件
- **Python 3.11+** 及 pip
- **Quarto** 用于文档渲染
- **基本 Python 包**：
  ```bash
  pip install pandas numpy matplotlib seaborn plotly requests beautifulsoup4 selenium
  ```

## 🛠️ 技术栈

- **Python 3.11+**：核心编程语言
- **Quarto**：技术内容发布系统
- **Pandas**：数据操作库
- **NumPy**：数值计算
- **Matplotlib/Seaborn**：数据可视化
- **Plotly**：交互式可视化
- **Requests/BeautifulSoup**：网络爬虫库
- **Selenium**：浏览器自动化
- **Jupyter**：交互式计算环境

## 📁 项目结构

```
Into-Python/
├── intro/                  # 介绍和基础
├── data manipulation/      # 数据分析库
├── plot/                   # 可视化库
├── Publish/                # 发布工具
├── other/                  # 高级主题
├── docs/                   # 渲染的 HTML 网站
├── _quarto.yml            # Quarto 配置
├── styles.css             # 自定义样式
├── foldableCodeBlock.lua  # 自定义 Quarto 过滤器
└── CLAUDE.md              # 开发指南
```

## 🔧 开发

### 构建网站
```bash
# 渲染整个网站
quarto render

# 实时预览
quarto preview

# 渲染特定文件
quarto render path/to/file.qmd
```
