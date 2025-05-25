# eCommerce Bolt Project

## Cloudflare Pages 部署指南

### 前置要求
- Cloudflare 账号
- 已连接 GitHub 仓库

### 部署步骤
1. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com)
2. 选择 "Pages" → "Create a project"
3. 选择你的 GitHub 仓库: `ecommerce_bolt_new_cline_gemini_2.5`
4. 配置构建设置:
   - **构建命令**: `npm run build`
   - **构建输出目录**: `dist`
5. 点击 "Save and Deploy"

### 环境变量配置（如需）
1. 在项目设置 → "Environment variables" 添加
2. 格式: `VITE_APP_VAR_NAME=value`

### 自定义域名
1. 在 "Custom domains" 添加你的域名
2. 按照提示配置 DNS 记录

### 注意事项
- 确保 `dist` 目录未被 .gitignore
- 静态资源请放在 `public` 目录
- 每次 git push 会自动触发部署

## 本地开发
```bash
npm install
npm run dev
```
