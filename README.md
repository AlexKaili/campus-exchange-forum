<div align="center">
<img src="https://github.com/user-attachments/assets/8919eace-b8a9-4775-b214-4656a96775df" width="80" height="80" alt="logo" />


# 校园交流论坛

**基于 Flask 的现代化全栈校园社区系统**

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-3.0-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-3.x-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![Alpine.js](https://img.shields.io/badge/Alpine.js-3.x-8BC0D0?style=flat-square&logo=alpinedotjs&logoColor=white)](https://alpinejs.dev)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

[功能特性](#-功能特性) · [技术栈](#-技术栈) · [快速开始](#-快速开始) · [项目结构](#-项目结构) · [截图预览](#-截图预览)

</div>

---

## 📖 项目简介

校园交流论坛是一个基于 **Python Flask** 开发的全栈社区系统，采用毛玻璃（Glassmorphism）设计风格，前后台功能完整，支持 PC 与移动端自适应，内置 WebSocket 实时通知。

适用于：**课程设计 / 毕业设计 / 个人学习 / 二次开发**


---

## ✨ 功能特性

### 前台功能

| 功能 | 说明 |
|------|------|
| 用户系统 | 注册（图形验证码）/ 登录 / 退出，本地头像上传 |
| 帖子管理 | 发布、浏览、编辑、删除，支持图片上传插入 |
| 互动功能 | 点赞、评论、二级回复（@用户名）、浏览量统计 |
| 版块分类 | 学习互助 / 项目组队 / 跳蚤市场 / 吃喝玩乐 / 失物招领 |
| 实时通知 | WebSocket 推送新评论 / 回复 / 点赞，铃铛角标实时更新 |
| 搜索功能 | 关键词搜索帖子与用户 |
| 个人主页 | 编辑资料、管理自己的帖子、查看获赞数 |
| 主题切换 | 亮色 / 暗色模式，浏览器本地持久化 |
| 响应式 | PC / 平板 / 手机端完全自适应 |

### 后台管理（`/admin`）

| 功能 | 说明 |
|------|------|
| 数据看板 | 用户数、帖子数、评论数、点赞数、今日新增统计 |
| 用户管理 | 搜索、封禁 / 解封、认证标识、删除 |
| 帖子管理 | 关键词搜索、版块筛选、查看、删除 |
| 评论管理 | 关键词搜索、删除 |

### 项目预览
电脑端 前台登录：
![1_前台登录](https://github.com/user-attachments/assets/63ebf01c-347f-4efc-ba66-25f3ed3e2068)、

手机端前台登录：
![1_前台登录_手机](https://github.com/user-attachments/assets/bfc4ce2c-d7b6-4e0e-90bc-dbed94d2115f)
![2_首页_pc](https://github.com/user-attachments/assets/0b01f62c-1c44-41f4-956e-2df24cae6ecb)

![2_首页_暗黑_pc](https://github.com/user-attachments/assets/af529af5-c301-4f4c-aa2b-4e20d573d64c)
![2_首页_暗黑_手机](https://github.com/user-attachments/assets/48bee00e-be90-4cfd-baaf-339ef8677d8d)

![3_帖子详情页_浅色_pc](https://github.com/user-attachments/assets/b23b846b-fa15-43c0-89a0-9ae33549b59c)
![4_个人主页](https://github.com/user-attachments/assets/9c087491-cf23-4f89-801e-b10678cab624)
![6_发布帖子](https://github.com/user-attachments/assets/688ff382-3577-438f-869a-c7ed99d5fa6c)

![7_管理后台_仪表盘](https://github.com/user-attachments/assets/aab2a2f5-19b6-40c1-8504-05058ee2b0ab)
![8_管理后台_帖子管理](https://github.com/user-attachments/assets/c84a9a83-778e-4ade-ba84-3b564b7a93a1)
![9_后台管理_评论管理](https://github.com/user-attachments/assets/885569fd-c1b5-4a72-8506-bd6b8d41cdfe)

---

## 🛠 技术栈

**后端**

- [Flask 3.0](https://flask.palletsprojects.com) — Web 框架
- [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com) — ORM
- [Flask-Login](https://flask-login.readthedocs.io) — 用户认证
- [Flask-SocketIO](https://flask-socketio.readthedocs.io) — WebSocket 实时通信
- [Pillow](https://pillow.readthedocs.io) — 图形验证码生成
- SQLite — 轻量级数据库

**前端**

- [Tailwind CSS](https://tailwindcss.com) — 原子化 CSS 框架
- [Alpine.js](https://alpinejs.dev) — 轻量级响应式框架
- [Socket.IO](https://socket.io) — 客户端实时通信
- [Font Awesome 6](https://fontawesome.com) — 图标库

---

## 🚀 快速开始

### 环境要求

- Python 3.8+
- pip

### 安装与运行

```bash
# 1. 解压压缩包
进入解压后的项目目录

# 2. 安装依赖
pip install -r requirements.txt

# 3. 启动应用
python app.py
```

浏览器访问 **http://127.0.0.1:5000** 即可。

> 首次启动会自动创建数据库并填充示例数据，无需手动操作。

### 默认账号

| 账号 | 密码 | 角色 |
|------|------|------|
| `CodeCraft` | `123456` | 管理员（可登录后台 `/admin/login`） |
| `小明` | `123456` | 普通用户 |

---

### 购买方式
微信：come6614
![二维码](https://github.com/user-attachments/assets/c9d04ab0-83dc-49d6-afc9-f5416f4decf3)


### 在线体验网址

前台：codemart.vip:5000

后台管理：codemart.vip:5000/admin/login

| 账号 | 密码 | 角色 |
|------|------|------|
| `小明` | `123456` | 普通用户 |
| `CodeCraft` | `123456` | 管理员|

