# 读书笔记

## Week 01 熟悉开发环境

这里我们使用 *Anaconda* 作为开发环境。首先需要去官网下载并安装 [Anaconda](https://www.anaconda.com/products/individual)，然后解压安装。

这里我们需要掌握如何通过 terminal 直接启动 jupyter (一个 IDE)。

```shell
cd Desktop
mkdir python_bootcamp
cd python_bootcamp
# 这里使用 jupyter notebook 启动 jupyter 的环境。其中 notebook 是一个执行参数，并不是文件名。
jupyter notebook
```

启动完 jupyter 后，会在当前路径下构建IDE环境。然后新建并重命名文件名为 *week_01*。然后掌握如何在 cell 中输入代码和markdown。
另外需要掌握显示 cell 中的行号。一个cell中可以输入多行代码，并作为一个执行单元。

> 如何显示行号

在cell的左侧空白单击然后按下键盘的 **L**键，不区分大小写。

> 使用 jupyter 快速编辑的技巧

当输入一行代码的时候， *ctrl+e* 切换到行位，然后回车换行。 *shift+回车* 执行代码。

> 如何使用占位符对齐

- str.ljust
- str.rjust
- str.center

```python3
# msg is "A****"
msg = str.ljust("A", 5, "*")
```

## week 06

frozenset 是一个不可变的 set。

```python3
fset = frozenset([1,2,3])
print(typeof(fset))
```

打开文件的不同模式（mode）

    - "r" This is the default mode. Open a file for reading only.
    - "w" Open a file for writing, If file does not exist. create it.
    - "x" create a new file, If file exists, the operation fails
    - "a" open in append mode. If file does not exist, create it.
    - "b" open in binary mode.
    - "+" will open a file for reading and writing. Good for updating
