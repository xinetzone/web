# Web

使用 Django 创建实用工具。

## 创建网站

Django 使您可以更轻松地以更少的代码更快地构建更好的 Web 应用程序。详细见官方教程 [Django3.1 文档](https://docs.djangoproject.com/zh-hans/3.1/)。

1. 启动项目

```sh
$ django-admin startproject dao
$ cd dao
```

2. 初始化一个投票应用

```sh
$ python manage.py startapp polls
```

3. 初始化迁移

```sh
$ python manage.py migrate
```

4. 修改设定后，再次更新迁移
    - 编辑 `models.py` 文件，改变模型。
    - 运行 `python manage.py makemigrations` 为模型的改变生成迁移文件。
    - 运行 `python manage.py migrate` 来应用数据库迁移。

5. 创建一个管理员账号

```sh
$ python manage.py createsuperuser
```

5. 启动服务器

```sh
$ python manage.py runserver
```