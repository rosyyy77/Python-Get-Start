# Python Basics

### Interpreter and Compiler

Interpreter (解释器) is a computer program that directly executes, instructions written in a programming or scripting language, without previously compiling them into a machine language program.

A compiler (编译器) is a computer program (or a set of programs) that transforms source code written in a programming language (the source language) into another computer language (the target language), with the latter often having a binary form known as object code.

### **Interactive v.s. script**

**Interactive**

✓ You type directly to Python one line at a time and it responds.

**Script**

✓ You enter a sequence of statements (lines) into a file using a text editor and tell Python to execute the file.

在Python编程中，注释和文档字符串（docstring）用于解释代码的功能、用途和实现细节。它们对于代码的可读性和维护性非常重要。以下是Python中行注释、块注释和docstring的详细解释：

### 行注释（Single-line Comments）

行注释用于在代码中添加简短的注释，通常放在一行代码的末尾或独立成行。行注释以 `#` 开头，后面的内容会被解释器忽略。

```python
# 这是一个行注释
x = 10  # 给变量 x 赋值
```

### 块注释（Block Comments）

块注释用于添加多行注释，可以是多个行注释组合在一起。块注释通常用于对较长或复杂的代码片段进行详细说明。

```python
# 这是一个块注释的第一行
# 这是块注释的第二行
# 这是块注释的第三行
for i in range(5):
    print(i)
```

### 文档字符串（Docstring）

文档字符串是用于为模块、类和函数等编写文档的字符串。文档字符串使用三重引号（`"""` 或 `'''`）包围，可以是单行或多行。文档字符串通常在模块、类或函数的开头，用于描述其功能和用途。

#### 模块文档字符串
```python
"""
这个模块提供了基本的数学运算功能。
包括加法、减法、乘法和除法。
"""

def add(a, b):
    """返回 a 和 b 的和。"""
    return a + b
```

#### 类文档字符串
```python
class MyClass:
    """
    这个类演示了一个简单的类定义。
    它包含一个方法用于打印问候语。
    """

    def greet(self):
        """打印问候语。"""
        print("Hello, World!")
```

#### 函数文档字符串
```python
def multiply(a, b):
    """
    返回 a 和 b 的乘积。

    参数:
    a -- 第一个乘数
    b -- 第二个乘数

    返回值:
    a 和 b 的乘积
    """
    return a * b
```

### 总结

- **行注释**：使用 `#`，用于单行简短注释。
- **块注释**：多个行注释组合，用于对较长或复杂代码片段进行详细说明。
- **文档字符串**：使用三重引号，用于模块、类和函数的文档说明，帮助生成自动化文档和提供开发者使用帮助。

使用合适的注释和文档字符串，可以极大地提高代码的可读性和可维护性，方便自己和他人理解和使用代码。