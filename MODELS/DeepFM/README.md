# DeepFM Model

## train.py
version 0.1

### TODO
- MLflow tracking setting
- Config 사용 설정
- dataset 완성 후 실험
- model 사용에 일반화

### RUN
> python train.py  

- Run with Argument option
> python train.py --optimizer Adam \\
                  --model DeepFM \\
                  --epochs 100 \\
                  ...
- Run with config  
-> 구현 예정
> python train.py --config True \\ 
                  --path ./config.json

### Argument

|option| default | Description
|------|:------:|------|
|seed|42| random seed|
|epoch|100| epoch|
|batchsize|1024| batch size|
|dataset|#TODO | dataset name|
|model|DeepFM| model name|
|optimizer|Adam| optimizer name|
|scheduler|StepLR| scheduler|
|lr_decay_step|50| StepLR 반감기|
|early_stopping|10| early stopping step size|
|lr|1e-2| learning rate|
|drop_rate|0.1|drop_rate|
|val_ratio|0.2|validation data ratio|
|criterion|cross_entropy|loss function|
|embedding_dim|10|embedding dimention|
|name|experiment| model expriment name|
    