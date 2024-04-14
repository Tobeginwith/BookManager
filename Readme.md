

### 功能介绍

平台采用B/S结构，后端采用Django框架进行开发，前端采用主流的Vue.js进行开发。

整个平台包括前台和后台两个部分。

- 前台功能包括：首页、图书详情页、用户中心模块。
- 后台功能包括：总览、借阅管理、图书管理、分类管理、标签管理、评论管理、用户管理、运营管理、日志管理、系统信息模块。

### 代码结构

- bookproject目录是后端代码
- web目录是前端代码

### 部署运行

#### 后端运行步骤

(1) 安装python 3.8

(2) 安装依赖。进入bookproject目录下，执行 pip install -r requirements.txt

(3) 安装mysql 5.7数据库，并创建数据库，命名为book，创建SQL如下：
```
CREATE DATABASE IF NOT EXISTS book DEFAULT CHARSET utf8 COLLATE utf8_general_ci
```
(4) 迁移数据。在bookproject目录下依次执行如下命令：

```
python manage.py makemigrations
python manage.py migrate
python manage.py makemigrations myapp
python manage.py migrate myapp
```

(5) 启动django服务。在bookproject目录下执行：
```
python manage.py runserver
```

#### 前端运行步骤

(1) 安装node 16.14

(2) 进入web目录下，安装依赖，执行:
```
npm install 
```
(3) 运行项目
```
npm run serve
```


### 界面预览

首页

![首页](https://raw.githubusercontent.com/geeeeeeeek/book/master/bookproject/upload/img/a.png)

后台首页

![后台首页](https://raw.githubusercontent.com/geeeeeeeek/book/master/bookproject/upload/img/b.png)

后台借阅管理

![后台借阅管理](https://raw.githubusercontent.com/geeeeeeeek/book/master/bookproject/upload/img/c.png)


### 待完善功能

- 邮箱推送功能
- 手机号绑定功能
- 粉丝关注功能

