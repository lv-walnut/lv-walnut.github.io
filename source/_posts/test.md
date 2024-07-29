---
title: test
date: 2024-07-24 16:08:37
tags:
---
# OS & Path
path通常用于表示文件路径或目录路径。您可以使用Python标准库中的os模块和pathlib模块来处理路径。

os模块提供了许多用于处理文件和目录的功能，包括创建、删除、重命名和移动文件或目录等。可以使用os.path模块中的函数来处理路径，例如：

python
Copy code
import os

# 获取当前工作目录
current_dir = os.getcwd()
print(current_dir)

# 获取文件名和路径
file_path = '/path/to/myfile.txt'
dir_path, file_name = os.path.split(file_path)
print(dir_path)
print(file_name)

# 检查文件或目录是否存在
file_exists = os.path.exists(file_path)
dir_exists = os.path.exists(dir_path)
print(file_exists)
print(dir_exists)
pathlib模块提供了更加面向对象的方式来处理路径，可以使用Path类来表示路径，并使用它的方法来处理路径。例如：

python
Copy code
from pathlib import Path