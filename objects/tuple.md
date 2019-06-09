### 元组tuple

元组是一个有序的元素组成的集合, 使用() 表示, 元组是不可变对象.

元组的定义 初始化

定义:

```
tuple()
t = tuple()
t = ()
t = tuple(range(1, 2, 3))
t = (1, 2, 3)
t = (1,)
t = (1,)*5
t = (1, 2, 3) * 6
```

元组元素的访问.

支持索引(下标).

正索引:从左至右, 从0开始, 为列表中每一个元素编号

负索引:从右至左, 从-1开始.

正负索引不可以超界, 否则引发异常indexError.

元组通过索引访问.

tuple[index], index 就是索引, 使用中括号访问.

```
t[1]

t[-2]

t[1]
```

### 元组查询

index(value,[start, [stop]]).

通过值value, 从指定区间查找列表内的元素是否匹配.

匹配第一个就立即返回索引.

匹配不到, 抛出异常ValueError.

count(value).

返回列表中匹配value的次数.

时间复杂度.

```
index和count方法都是O(n)

随着列表数据规模的增大,而效率下降
```

len(tuple): 返回元素的个数.

### 元组的其他操作

元组是只读的, 所以增, 改 ,删方法都没有.