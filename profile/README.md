# 团队公约
---

## 🧐 介绍
西安电子科技大学-智能媒体计算实验室-多视角深度学习研究团队

## 📁 仓库约定

**仓库命名**
以论文中提及的模型简称为准

**仓库文件结构**
以[xdmvteam/TMC](https://github.com/xdmvteam/TMC)为模板

## 🔤 数据集预处理约定

多视角python数据格式约定：
```python
[
    # dict key 表示视角编号；array(...)代表该视角的样本列表,形状为(num_samples, ...)
    {0:[array(...), array(...), ...], 1:[array(...), array(...), ...], ...},
    [int, int, ...]  # 每个样本的标签
]
```
对于多视角数据集，不论来源，不论格式，一律预处理为上述python格式，训练、测试、验证集分别保存为文件。

预处理方式可参考[xdmvteam/TMC/dataset](https://github.com/xdmvteam/TMC/tree/main/dataset)。
