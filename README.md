# AI超级个体俱乐部 - ChatGPT UI

一个高保真还原 ChatGPT 网页界面的项目，集成了 AI超级个体俱乐部会员弹窗。

## 项目结构

```
AIw2026/
├── chatgpt-ui.html      # 主页面 - ChatGPT UI + 弹窗
├── modal-template.html  # 弹窗模板文件
├── 223510.png          # 支付二维码图片
└── README.md           # 项目说明
```

## 功能特性

### ChatGPT UI
- 顶部导航栏（Logo、产品名称、登录/注册按钮）
- 侧边栏（对话历史、新建对话按钮、用户菜单）
- 主内容区域（欢迎标题、智能输入框）
- 功能按钮（附件、搜索、学习、创建图片、语音）
- 消息气泡（用户和AI的消息区分）
- 设置面板模态窗口
- 完全响应式设计（桌面端和移动端适配）

### AI超级个体俱乐部弹窗
- 全局锁定：页面加载后自动弹出，背景模糊锁定
- 防关闭机制：点击遮罩和ESC键无法关闭（震动提示）
- 春节特惠：仅需3.99元
- 支付二维码展示
- 完全响应式（支持小屏手机、平板、桌面端）

## 使用方法

### 本地预览
```bash
python -m http.server 8080
```
然后访问 http://localhost:8080/chatgpt-ui.html

### 部署到 Cloudflare Pages
本项目已配置 GitHub Actions，推送到 main 分支后会自动部署到 Cloudflare Pages。

## 技术栈
- HTML5
- CSS3 (Flexbox, Grid, 媒体查询)
- JavaScript (原生)

## 响应式断点
- 小屏手机: <= 375px
- 手机: 376px - 767px
- 平板: 768px - 1023px
- 桌面: >= 1024px

## 许可证
MIT License
