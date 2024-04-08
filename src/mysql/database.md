## Database

### 查询

```sql
# 查询所有数据库
show databases;

# 查询当前数据库
select database();
```

### 使用

```sql
use 数据库名;
```

### 创建

```sql
create database [if not exists] 数据库名;
```

### 删除

```sql
drop database [if exists] 数据库名;
```