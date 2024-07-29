---
title: about
date: 2024-07-24 16:52:25
---
# 获取当前工作目录
current_dir = Path.cwd()
print(current_dir)

# 获取文件名和路径
file_path = Path('/path/to/myfile.txt')
dir_path, file_name = file_path.parent, file_path.name
print(dir_path)
print(file_name)

# 检查文件或目录是否存在
file_exists = file_path.exists()
dir_exists = dir_path.exists()
print(file_exists)
print(dir_exists)

