# 基于train_s3dis_v13.py

# 目录结构
```shell
WS3
├── data               # 数据集的处理
│── model              # 网络模型
|── utils                             
│  ├── cpp_wrappers
│  ├── meta
│  ├── nearest_neighbors
│  ├── ...
|  └── tools.py
|
|── train.py            # 线下模型训练
|── test.py             # 模型测试
└── train_modelarts.py  # modelarts训练作业的启动入口
```

# 数据集S3DIS



# 本地GPU训练
```shell
python train.py --device_target GPU
```


# 线上GPU训练
## 启动文件
```shell
train_modelarts.py
```
## 在ModelsArts上训练的注意事项
1. 第三方库需要指定版本: requirements.txt (限定scikit-learn==0.21.3)
2. 安装nearest_neighbors: train_modelarts.py中需要执行shell script (包含cd utils/nearest_neighbors & python setup.py develop)
