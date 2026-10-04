# EasyEnglish Learning App - MVP

一个为中初中学生设计的英语学习移动应用，包含词汇、语法、听力、阅读等核心功能。

## 📋 项目概述

**应用名称**: EasyEnglish Learning  
**目标用户**: 中学/初中生  
**核心特性**:
- 📚 词汇学习（含图片、发音、例句）
- 📖 语法训练（含讲解和练习题）
- 🎧 听力练习（分级对话）
- 📝 阅读理解（分级短文）
- 🎤 口语跟读（基础发音训练）
- ✍️ 写作辅助（句型模板）
- 🏆 打卡激励（积分、徽章、排行榜）
- 📊 错题本（自动分类复习）

## 📁 项目结构

```
EasyEnglish-Learning-App/
├── frontend/                 # Flutter 前端应用
│   ├── lib/
│   │   ├── main.dart
│   │   ├── screens/
│   │   ├── models/
│   │   ├── services/
│   │   └── widgets/
│   ├── pubspec.yaml
│   └── README.md
├── backend/                  # Node.js 后端服务
│   ├── src/
│   │   ├── server.js
│   │   ├── routes/
│   │   ├── controllers/
│   │   ├── models/
│   │   └── middleware/
│   ├── package.json
│   └── README.md
├── database/                 # 数据库设计
│   ├── schema.sql
│   └── seed_data.sql
├── docs/                     # 项目文档
│   ├── API_DOCUMENTATION.md
│   ├── DATABASE_DESIGN.md
│   └── ARCHITECTURE.md
└── README.md
```

## 🚀 快速开始

### 前置要求
- Node.js 14+ 和 npm
- Flutter SDK
- MySQL 5.7+
- Git

### 后端启动

```bash
cd backend
npm install
npm start
# 服务运行在 http://localhost:3000
```

### 前端启动

```bash
cd frontend
flutter pub get
flutter run
```

## 📱 核心功能

### 1. 首页 (Home Screen)
- 今日任务卡片
- 学习进度条
- 连续打卡信息
- 推荐学习内容

### 2. 词汇学习 (Vocabulary Module)
- 单词卡片浏览
- 图片+释义+例句
- 发音播放
- 单词测试
- 复习列表

### 3. 语法训练 (Grammar Module)
- 语法点讲解
- 例题示范
- 练习题（单选/多选）
- 详细解析
- 错题记录

### 4. 听力练习 (Listening Module)
- 对话播放
- 字幕显示
- 理解题目
- 逐句重放
- 语速调节

### 5. 阅读理解 (Reading Module)
- 分级阅读材料
- 关键词高亮
- 理解题目
- 词汇注解
- 阅读统计

### 6. 口语跟读 (Speaking Module)
- 短句播放
- 用户录音
- 简单打分
- 重复练习
- 进度跟踪

### 7. 打卡激励 (Gamification)
- 每日打卡
- 积分系统
- 成就徽章
- 排行榜
- 周报告

### 8. 错题本 (Mistakes Tracking)
- 自动收录错题
- 分类统计
- 重点复习
- 进度对比

## 🛠 技术栈

**前端**:
- Flutter (Dart)
- Provider 状态管理
- HTTP 网络请求
- SQLite 本地存储

**后端**:
- Node.js + Express
- MySQL 数据库
- JWT 认证
- RESTful API

**其他**:
- 发音 API（讯飞/百度）
- 语音识别（可选）
- 推送通知

## 📚 API 端点示例

| 功能 | 方法 | 端点 |
|------|------|------|
| 登录 | POST | `/api/auth/login` |
| 获取词汇列表 | GET | `/api/vocabulary/list` |
| 提交语法答案 | POST | `/api/grammar/submit` |
| 获取听力材料 | GET | `/api/listening/:id` |
| 获取阅读内容 | GET | `/api/reading/:id` |
| 提交口语录音 | POST | `/api/speaking/submit` |
| 获取打卡信息 | GET | `/api/checkin/status` |
| 获取错题本 | GET | `/api/mistakes/list` |

## 🗄 数据库设计概览

**核心表**:
- `users` - 用户信息
- `vocabulary` - 词汇库
- `grammar_points` - 语法点
- `listening_materials` - 听力素材
- `reading_materials` - 阅读材料
- `user_progress` - 学习进度
- `mistakes` - 错题记录
- `achievements` - 成就徽章
- `daily_checkin` - 打卡记录

详见 `database/schema.sql`

## 📊 学习路径

**基础层**（一级用户）:
- 每日：10 个词汇 + 1 个语法点 + 1 段听力

**提升层**（二级用户）:
- 每日：15 个词汇 + 2 道语法题 + 1 段听力 + 1 篇阅读

**强化层**（三级用户）:
- 每日：20 个词汇 + 语法 + 听力 + 阅读 + 口语 + 复习错题

## 🎯 MVP 优先级

**Phase 1** (核心功能):
- [ ] 用户认证与登录
- [ ] 词汇学习与测试
- [ ] 语法题练习
- [ ] 错题本
- [ ] 打卡系统

**Phase 2** (扩展功能):
- [ ] 听力练习
- [ ] 阅读理解
- [ ] 成就徽章系统
- [ ] 排行榜

**Phase 3** (高级功能):
- [ ] 口语跟读与评分
- [ ] 写作辅助
- [ ] AI 纠错
- [ ] 社交分享

## 📖 文档

- [API 文档](./docs/API_DOCUMENTATION.md)
- [数据库设计](./docs/DATABASE_DESIGN.md)
- [架构设计](./docs/ARCHITECTURE.md)
- [前端 README](./frontend/README.md)
- [后端 README](./backend/README.md)

## 🤝 贡献指南

欢迎贡献代码、报告问题或提出功能建议！

## 📝 许可证

MIT License

## 👥 联系方式

如有问题或建议，请提交 Issue 或 Pull Request。

---

**最后更新**: 2026-10-04  
**版本**: 0.1.0-MVP
