![[截屏2023-08-01 14.10.22.png]]
	静态sql中，多个字段中每个字段都有可能进行更改

# 修改配置文件
	结合传递的数据进行动态语句的配置，使得某些条件满足时才出现特定查询语句

## if语句

### select 语句
![[截屏2023-08-01 14.14.07.png|500]]

#### 测试
![[截屏2023-08-01 14.15.41.png|675]]
	如果不设置任何条件或者设置多个条件，sql语句可能出现错误

### insert 语句
![[截屏2023-08-01 14.21.32.png|550]]

#### 测试
	数据的筛选从业务层到数据层中，设置条件

![[截屏2023-08-01 14.25.11.png]]

## choose语句
	类似于if-else 多条件判断，实现更加简化的处理
	通过choose实现不同的查询组合

### select where
![[截屏2023-08-01 14.27.49.png]]

**修改配置文件**

![[截屏2023-08-01 14.28.42.png|550]]
	修改不同条件下的默认值，可以在某些情况下不出现where子句——性能上得到改进
	otherwise 子句表示其他情况下代码输出的语句


## set语句
	动态设置更新字段的意思

#### 配置文件修改
![[截屏2023-08-01 14.37.22.png|675]]
	可以根据需要选择要更新的内容

![[截屏2023-08-01 14.41.11.png]]

## foreach语句
	循环语句操作，最重要在于删除操作

### 配置文件修改
![[截屏2023-08-01 14.43.36.png]]

### 测试
	使用set进行编号数据的传递

![[截屏2023-08-01 14.46.19.png]]

### 配置文件修改
	循环查询操作

![[截屏2023-08-01 14.48.32.png|600]]
### 测试

![[截屏2023-08-01 14.49.50.png|600]]

### 配置文件修改
	批处理

![[截屏2023-08-01 14.50.57.png|550]]
### 测试
![[截屏2023-08-01 14.51.47.png|550]]