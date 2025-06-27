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