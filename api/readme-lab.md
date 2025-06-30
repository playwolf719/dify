# 写在前面

- 基于dify的1.3.1做的修改


# 初始化

## env
```

cp .env.example .env 
```

## db
```
# 只记录，不执行
flask db migrate -m "Add metainfo column to Document table"
```


## docker image
```

# origin
registry-cn-hangzhou-vpc.ack.aliyuncs.com/acs/dify-api:1.3.1

# new
sudo docker build -t dify-api:szlab-v1.0 . && sudo docker tag dify-api:szlab-v1.0 crpi-7pbvq1eixd9nit76-vpc.cn-hangzhou.personal.cr.aliyuncs.com/szailab/dify-api:szlab-v1.0 && sudo docker push crpi-7pbvq1eixd9nit76-vpc.cn-hangzhou.personal.cr.aliyuncs.com/szailab/dify-api:szlab-v1.0

```