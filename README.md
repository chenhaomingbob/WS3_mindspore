# 基于train_s3dis_v13.py
# 在ModelsArts上训练的注意事项
1. 第三方库需要指定版本: requirements.txt (限定scikit-learn==0.21.3)
2. 安装nearest_neighbors: train_modelarts.py中需要执行shell script (包含cd utils/nearest_neighbors & python setup.py develop)
