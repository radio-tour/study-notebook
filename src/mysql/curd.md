## Curd

### 插入

- 指定字段添加数据 `insert into 表名

```sql
# 指定字段添加数据
insert into 表名(字段名, ...) values (值, ...);

# 全部字段添加数据
insert into 表名 values (值, ...);

# 批量添加数据（指定字段）
insert into 表名(字段名, ...) values (值, ...), (值, ...);

# 批量添加数据（全部字段）
insert into 表名 values (值, ...), (值, ...);
```

### 删除

```sql
# 删除所有数据
delete from 表名;

# 删除指定数据
delete from 表名 [where 条件];
```

### 更新

```sql
update 表名 set 字段名=值, ... [where 条件];
```