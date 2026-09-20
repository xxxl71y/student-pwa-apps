# 大学生 PWA 应用集

两个可安装的 PWA 应用，部署在 GitHub Pages 上，支持离线使用、安装到桌面/手机主屏。

## 应用列表

### 1. 大学生记账本

追踪每月收支，清楚钱花在哪。

- 添加收入/支出记录（金额、分类、备注、日期）
- 月度统计卡片（收入、支出、结余）
- 分类支出 SVG 饼图
- 月份切换浏览历史数据
- LocalStorage 本地持久化

**访问地址**: https://xxxl71y.github.io/student-pwa-apps/记账本/

### 2. DDL 倒计时看板

所有截止日期一目了然。

- 添加事件（名称、截止日期、分类）
- 倒计时卡片展示（还有 X 天）
- 紧急度颜色（≤3天红色 / ≤7天黄色 / >7天绿色）
- 按天数自动排序
- 过期事件标灰
- 分类筛选（考试/作业/活动/其他）
- LocalStorage 本地持久化

**访问地址**: https://xxxl71y.github.io/student-pwa-apps/倒计时看板/

## 技术栈

- 单 HTML 文件（HTML + CSS + 原生 JS）
- PWA（manifest.json + Service Worker）
- LocalStorage 数据存储
- SVG 图表（无外部依赖）
- GitHub Pages 自动部署

## 本地使用

用 Python 启动本地服务器：

```bash
cd student-pwa-apps
python -m http.server 8000
```

浏览器访问 http://localhost:8000/记账本/ 或 http://localhost:8000/倒计时看板/

## 安装为 App

在 Chrome/Edge 中打开应用页面，点击地址栏右侧的"安装"按钮，即可安装到桌面，像原生 App 一样使用。
