# 基于train_s3dis_v13.py
# 在ModelsArts上训练的注意事项
1. requirements.txt (限定scikit-learn==0.21.3)
2. 在train_xx.py中执行shell script (包含python setup.py develop), 从而来安装nearest_neighbors
3. GatherD的index类型都通过astype改为int32