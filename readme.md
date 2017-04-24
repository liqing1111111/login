## 数据库

#### SQL查询语句

###     先说增删改:

### 增,就是insert into:

```
   INSERT INTO 表明 (字段1,字段2..) VALUES (值1, 值2...)
例子:
   INSERT INTO user(name,sex,age) VALUES ("于","30","男")
```

### 删,就是delete:

```
  delete from 表名 WHERE 条件1 and 条件2 
例子:
DELETE FROM USER WHERE id = 1

同时满足两个条件:
DELETE FROM USER WHERE sex = "女" AND age > 30
```





### 改,就是update:

```
UPDATE   表名 set  字段1 = 值 1,字段2 = 值2 where 条件
例子:
   UPDATE USER SET name = "a",age = 18 WHERE id = 10
```



### 查



### 查,就是select:

```
 
 SELECT 字段名 FROM 表名 where 条件
 
 查找 所有数据
  SELECT * FROM USER
  有条件的查找 模糊查询
  SELECT * FROM USER WHERE name like "%小"
  
  排序 按照年龄降序排列  DESC   升序asc  默认是升序
  SELECT * FROM `USER` ORDER BY age DESC
  
  
  LIMIT从第几条数据开始查,查几条   从0开始数的
  
  SELECT * FROM USER LIMIT 2,3
```







