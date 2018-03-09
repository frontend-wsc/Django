## 快速搭建 Django 开发环境
 * 第1步 安装 python，这里我推荐搭建下载python3	[https://www.python.org/](https://www.python.org/ "python 官网")
 
       检测是否安装成功 cmd 终端  运行 python  --version
 * 第2步 检查本地是否下载了 Django package
      ```python
         python -m django --version
      ```
      如果终端输出如 2.0.3 说明已经安装了 Django，反之安装 django 2.0
      ```python
      pip install django
      ```
  
##Creating a project
 ```
 	$ django-admin startproject mysite
 ```