# ChemThermo Pro v4.0 - 部署指南

## 方案A: Vercel部署（推荐，最简单）

### 第1步：注册GitHub账号
1. 打开 https://github.com （如已有账号跳过）
2. 点击 "Sign up" 注册
3. 验证邮箱

### 第2步：上传项目到GitHub
1. 登录GitHub后，点击右上角 "+" → "New repository"
2. 输入仓库名：chemthermo-pro
3. 选择 "Public"
4. 点击 "Create repository"
5. 点击 "uploading an existing file"
6. 把本文件夹中的所有文件拖拽上传：
   - package.json
   - vite.config.js
   - index.html
   - src/main.jsx
   - src/App.jsx
7. 点击 "Commit changes"

### 第3步：Vercel部署
1. 打开 https://vercel.com
2. 点击 "Sign Up" → 用GitHub账号登录
3. 点击 "Add New Project"
4. 选择你刚创建的 chemthermo-pro 仓库
5. Framework Preset 选择 "Vite"
6. 点击 "Deploy"
7. 等待约1分钟，部署完成！
8. 你会得到一个链接如 chemthermo-pro.vercel.app

### 第4步（可选）：绑定自定义域名
1. 在阿里云/腾讯云购买域名（如 chemthermo.cn，约60元/年）
2. 在Vercel项目设置 → Domains → 添加你的域名
3. 按照提示配置DNS记录

## 方案B: 任何静态服务器

如果你有自己的服务器或虚拟主机：
1. 在本地安装 Node.js (https://nodejs.org)
2. 在项目目录运行：
   npm install
   npm run build
3. 把 dist/ 文件夹的内容上传到你的服务器

## 文件说明

```
chemthermo-pro/
├── index.html          入口HTML页面
├── package.json        项目配置和依赖
├── vite.config.js      构建工具配置
├── README.md           本说明文件
└── src/
    ├── main.jsx        React入口
    └── App.jsx         ChemThermo Pro主程序（1956行）
```

## 技术栈
- React 18
- Recharts (图表库)
- Vite (构建工具)
- 纯前端，无需后端服务器

## 联系
chemthermo@outlook.com
