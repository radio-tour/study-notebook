## 查询

### 基础语法

注意：查询结果也是一个二维表，它包含列名和每一行的数据。

```sql
# 通用
select
  字段列表
from
  表名列表
where
  条件列表
group by
  分组字段列表
having
  分组后条件列表
order by
  排序字段列表
limit
  分页参数;

# 简化
select 字段名, ... from 表名;
select * from 表名;
select 字段名 [as 别名], ... from 表名;
select distinct 字段列表 from 表名;
```