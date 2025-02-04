# 数据库大作业——2024 年春季

## 项目介绍

基于 `flask` 开发的影评平台，参考豆瓣和 IMDb。

## 项目结构

```bash
.
├── README.md
├── apps
│   ├── __init__.py
│   ├── config.py
│   ├── main
│   │   ├── __init__.py
│   │   └── view.py
│   ├── menu
│   │   ├── __init__.py
│   │   └── view.py
│   ├── movie
│   │   ├── __init__.py
│   │   └── view.py
│   └── user
│       ├── __init__.py
│       ├── module.py
│       └── view.py
├── assets
│   ├── css
│   │   └── base.css
│   └── js
│       └── base.js
├── data
│   ├── movies
│   │   └── imdb_top250.json
│   └── src
│       ├── main.py
│       └── module.py
├── extensions
│   ├── __init__.py
│   └── mysql
│       ├── __init__.py
│       └── module.py
├── requirements.txt
├── run.py
├── schema.sql
└── templates
    ├── base.html
    ├── main
    │   └── index.html
    ├── menu
    │   └── index.html
    └── user
        ├── login.html
        ├── profile.html
        └── register.html

17 directories, 29 files
```

## 项目运行

### 安装依赖

```bash
pip install requirements.txt
```

### 运行

```bash
python run.py -m develop
```

```bash
usage: run.py [-h] [-m MODE]

Run the web application.

options:
  -h, --help            show this help message and exit
  -m MODE, --mode MODE  Mode in which to run the app, MODE: default, develop, test
```

## 更新日志

- 2024-6-6：完成基础用户登陆验证模块，创建 IMDb 对象爬取 Top 25 的电影；
