# nyc-airbnb-price-analysis
An analysis of NYC Airbnb listing prices and their influencing factors.
# 🏠 纽约市 Airbnb 市场数据分析与定价策略研究

## 项目概述

本项目对纽约市2019年的Airbnb开放数据集进行了深入分析，旨在揭示影响房源定价的关键因素，并为房东提供数据驱动的定价策略建议。分析涵盖了描述性统计、数据可视化以及严格的统计假设检验。

- **数据集:** 包含48,895条房源记录，16个特征变量。
- **工具:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy
- **关键词:** `数据清洗` `可视化` `假设检验` `价格分析` `商业洞察`

## 核心研究问题

1.  纽约市不同行政区（如曼哈顿、布鲁克林）的Airbnb价格分布有何差异？
2.  不同的房间类型（整租、合租、共享房间）如何影响定价？
3.  用户评论数量与房源价格之间存在何种关系？

## 项目文件结构
nyc-airbnb-price-analysis/
├── NYC_Airbnb_Analysis.ipynb # 主分析笔记本（包含完整代码与报告）
├── README.md # 本项目说明文件

## 主要分析步骤与发现

1.  **数据预处理:** 处理了缺失值，并聚焦于核心变量（ neighbourhood_group, room_type, price等）。
2.  **描述性统计与可视化:**
    - 价格呈高度右偏分布，存在极端异常值。
    - **曼哈顿**的平均价格最高（$196），**布朗克斯**最低（$87）。
    - **整租房源**的价格远高于其他类型。
3.  **假设检验:**
    - **Kruskal-Wallis H检验:** 证实了不同行政区之间的价格中位数存在**极其显著的差异**（p < 0.05）。
    - **Pearson相关性检验:** 发现评论数量与价格之间存在**微弱但显著的负相关**（r = -0.048, p < 0.05）。

## 核心结论与商业建议

-   **地理位置优先:** 定价策略应首要考虑房源所在的行政区。
-   **房间类型是关键:** 整租房源可制定溢价策略。
-   **平衡定价与需求:** 价格过高可能会抑制订单量和评论增长，房东需在两者间找到平衡。

## 作者

**Fiona Zi**
- 邮箱：fionaz12308@gmail.com

## 致谢

- 数据来源：New York City Airbnb Open Data[https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data]

