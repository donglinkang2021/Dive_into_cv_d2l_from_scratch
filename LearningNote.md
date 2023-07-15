# 记录学习笔记

> 学海无涯，快快乐乐

## python在字符串前面加个f或者r是什么意思呢（gpt answer）

在Python中，前缀为`f`或`r`的字符串被称为“f-string”和“raw string”，它们分别表示以下内容：

1. `f-string`: 在字符串前添加`f`前缀，可以在字符串中使用花括号`{}`来插入变量或表达式的值。Python会在运行时计算花括号中的表达式，并将其结果插入到字符串中。例如：

```python
name = "Alice"
age = 25
message = f"My name is {name} and I am {age} years old."
print(message)  # 输出："My name is Alice and I am 25 years old."
```

2. `raw string`: 在字符串前添加`r`前缀，表示这个字符串是“原始字符串”，即字符串中的反斜杠`\`不会被特殊处理。这通常用于处理正则表达式、文件路径等包含反斜杠的字符串。例如：

```python
path = r"C:\Users\Alice\Documents"
print(path)  # 输出："C:\Users\Alice\Documents"
```

需要注意的是，`f-string`和`raw string`只是一种语法糖，不会改变字符串本身的类型或性质。在使用时需要根据具体的需求来选择是否使用这些前缀。

## 学习这一章中的小心得（乘着烤机的时候来写点东西）

### metric

李沐的书里加入了metric一个自定义的Accumulater的类来记录每一个epoch中的累加评判指标，到最后又统一由这个类来计算出一个平均值，再把每个epoch中的metric加入自己的animator类中，动态展示训练的整个过程，这种思路自己在学习完了面向对象和android开发才更好的体会到这种程序设计的魅力，受益良多。

## 理解.contiguous()的作用

[参考这里](https://stackoverflow.com/questions/48915810/what-does-contiguous-do-in-pytorch)