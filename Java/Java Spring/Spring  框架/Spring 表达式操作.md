# 基本操作
![[截屏2023-07-17 11.49.05 2.png]]
# 作用原理
![[截屏2023-07-17 13.05.42.png]]
# 自定义EL表达式分隔符
自动转型

# 数学运算

# 逻辑运算

## 普通逻辑运算

## 三目运算符

### 扩展

# Class 表达式
![[截屏2023-07-17 14.09.29.png]]
![[截屏2023-07-17 14.15.56.png]]
## 表达式变量

使用表达式代替的内容，类型随意

![[截屏2023-07-17 14.31.27.png]]
### 根变量
![[截屏2023-07-17 14.33.22.png]] 
#### 方法引用
![[截屏2023-07-17 14.35.35.png]]

#### 类属性方法引用
![[截屏2023-07-17 14.38.32.png]]
对象必须存在，否则异常。
**通过Groovy表达式进行处理**

#### 使用Grovvy表达式处理null
![[截屏2023-07-17 14.38.32 1.png]]
判断当前变量是否为空，空则返回null，否则按正常计算处理

# List 集合表达式
![[截屏2023-07-17 14.50.06.png]]
	集合要加大括号
## 集合相关操作

### 外部集合访问
![[截屏2023-07-17 14.52.04.png]]

### 修改索引所指位置

*listof* 生成的集合不可修改
![[截屏2023-07-17 14.54.02.png]]

### 修改整个集合数据
![[截屏2023-07-17 14.57.11.png]]
	不修改原集合，将修改后的数据保存到新集合中

# Map集合表达式
### get功能封装
![[截屏2023-07-17 15.07.38.png]]

### put操作
![[截屏2023-07-17 15.09.27.png]]
### Map转化为List

![[截屏2023-07-17 15.12.10.png]]
### 筛选

![[截屏2023-07-17 15.11.26.png]]

# 配置文件整合SpEL

# 使用注解SpEL
## @Value 直接在bean定义中赋值

## @Profile 结合SpEL
	初步具有实际意义
	
![[截屏2023-07-17 15.53.23 1.png]]


