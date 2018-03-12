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

## The development server
  * 启动一个 web 服务器
```
 	$ cd mysite
      python manager.py runserver
 ```

* 创建管理员
```
	python .\manage.py createsuperuser
```
* 配置应用
  - 在应用的admin.py中引入自身的models模块(或里面的类型类)
  - edit admin.py: admin.site.register(models.ClassName)
  - edit models.ClassName:
    	添加
        def __str__(self):
         return self.title
         修改数据展示形式