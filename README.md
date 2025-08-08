# 揭阳第一中学数模队官网

## 项目简介
**揭阳第一中学数模队官网** 是校队面向校内外的**官方展示与招新门户**。  
网站以「**Model the World, Code the Future**」为口号，一站式呈现：
- 16 位队干 3D 风采卡片
- 官方宣传片 & 宣传海报
- 品牌活动与荣誉奖项
- 完整队规与在线报名通道

> 页面采用**单文件静态设计**，无需打包即可直接部署；深色科技风 + AOS 动效，兼顾手机/电脑多端体验。

---

## 🚀 快速开始
1. **克隆 / 下载**  
   ```bash
   git clone https://github.com/Jessssssseea/JYYZMMC.git
   ```

2. **本地预览**  
   将仓库放在任意静态服务器（`Live Server`、`nginx`、`GitHub Pages` 等）即可。  
   或直接用浏览器打开 `index.html`（部分动效需 http 环境）。

---

## 🎨 技术栈
| 技术 | 用途 |
|---|---|
| **原生 HTML5 + CSS3** | 页面结构与样式 |
| **AOS 2.3.4** | 滚动动画库（CDN） |
| **原生 JavaScript** | 3D 翻转卡片、平滑滚动 |
| **CSS Grid / Flex** | 响应式布局 |
| **固定深色主题** | 赛博朋克风配色 `#0d1b2a` / `#00b4d8` |

---

## 📱 响应式特性
- **手机端**：导航自动换行、卡片单列、海报双列自适应。
- **桌面端**：最大宽度 1200 px，居中显示；3D 卡片悬停翻转。
- **首屏**：100 vh 背景固定，社徽随屏幕比例缩放。

---

## 🛠️ 二次开发指南
### 1. 更换资源
- **队干照片**：重命名并覆盖 `assets/images/leaders/姓名.jpg`  
  如需随机双图，在 `leaders` 数组里设置 `rand:true`。
- **宣传海报**：直接替换 `assets/images/*.png|jpg`。
- **宣传片封面**：替换 `assets/images/hero-poster.png`。

### 2. 颜色与字体
- 全局 CSS 变量在 `<style>` 头部：
  ```css
  :root {
    --bg:#0d1b2a;
    --card:#1b263b;
    --accent:#00b4d8;
    --text:#f1faee;
    --radius:12px;
    --font:'Segoe UI',sans-serif;
  }
  ```

### 3. 新增栏目
只需在 `<body>` 内按以下模板追加：
```html
<section id="new">
  <h2>新栏目标题</h2>
  <!-- 内容 -->
</section>
```
并在 `<nav>` 里补充锚点链接即可。

---

## 📄 许可证
MIT License – 允许二次创作与商业使用，请保留原作者署名。

---

## 📞 联系我们
- 咨询 QQ 群：103312220  
- 报名问卷：https://wj.qq.com/s2/23398546/ad18/  
- 邮箱：jess2285287248@gmail.com

---

**揭阳第一中学数模队 © 2025**  
让我们一起「用数学建模，丈量世界」。