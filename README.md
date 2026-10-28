# 基于注意力机制的AES能量迹侧信道攻击方法研究

大学生创新创业训练计划项目

## 项目成员
- 陈飞达（负责人）：模型搭建、项目统筹
- 肖钟麒：SE-Net注意力模块
- 伏起旺：数据加载、训练框架、评估指标
- 孙小涵：文献调研、可解释性分析

## 仓库结构

ascad-sidechannel/
├── data/               # 数据集（本地存放，不上传）
├── models/             # 神经网络模型
│   ├── baseline_cnn.py # 基准CNN
│   └── se_module.py    # SE-Net注意力模块
├── utils/              # 工具函数
│   ├── dataloader.py   # 数据加载
│   └── metrics.py      # 猜测熵等评估指标
├── visualize/          # Grad-CAM可视化
├── docs/               # 文献综述与文档
└── train.py            # 训练脚本


## 使用说明
1. 将 ASCAD.h5 数据集放入 `data/` 文件夹
2. 运行 `python utils/dataloader.py` 测试数据加载
3. 运行 `python models/baseline_cnn.py` 测试模型
