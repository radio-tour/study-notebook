## 表

### 约束

约束是作用于表中字段上的规则，用于限制表中的数据

| 关键字 | 约束 | 描述 |
| --- | --- | --- |
| not null | 非空约束 | 限制该字段值不能为 null |
| unique | 唯一约束 | 限制该字段值唯一不重复 |
| primary key [auto_increment] | 主键约束 | 主键是一行数据的唯一标识，要求非空且唯一 【自动向上增长】 |
| default 默认值 | 默认约束 | 保存数据时若未指定字段值，则采用默认值 |
| foreign key | 外键约束 | 让两张的数据建立连接 |

### 创建

```sql
create table 表名 {
  字段名 字段类型 [约束] [comment 字段注释],
  ...
} [comment 表注释];
```

### 查询

```sql
# 查询所有表
show tables;

# 查询指定表结构
desc 表名;

# 查询建表语句
show create table 表名;
```

### 修改

```sql
# 添加字段
alter table 表名 add 字段名 字段类型 [约束] [comment 注释];

# 修改字段类型
alter table 表名 modify 字段名 新类型;

# 修改字段名
alter table 表名 change 旧字段名 新字段名 类型 [约束] [comment 注释];

# 删除字段
alter table 表名 drop column 字段名;

# 修改表名
rename table 表名 to 新表名;
```