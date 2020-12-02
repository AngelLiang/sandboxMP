# 快速部署预览

## 创建数据库

    > mysql -u root -p
    mysql> CREATE SCHEMA `sandboxmp` DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_bin ;

## 导入初始数据

    mysql -uroot -p sandboxMP < config/basic_data_20190225.sql

## 创建环境

    pipenv install
    pipenv shell
    python manage.py runserver


- 默认管理员：admin
- 密码：1234@abcd.com

如果登录失败，可以修改默认管理员的密码

    python manage.py changepassword
